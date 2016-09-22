# calculator
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;



namespace WindowsFormsApplication1
{

    public partial class Form1 : Form
    {
        double number1;
        int pos;
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {

            addNum(1);
        }

        private void button5_Click(object sender, EventArgs e)
        {
            addNum(5);
        }

        private void button6_Click(object sender, EventArgs e)
        {
            addNum(6);
        }

        private void button4_Click(object sender, EventArgs e)
        {
            addNum(4);
        }

        private void textBox1_TextChanged(object sender, EventArgs e)
        { }
        public void addNum(int num)
        {
            textBox1.Text = textBox1.Text + num.ToString();

        }

        private void button2_Click(object sender, EventArgs e)
        {
            addNum(2);
        }

        private void button3_Click(object sender, EventArgs e)
        {
            addNum(3);
        }

        private void button7_Click(object sender, EventArgs e)
        {
            addNum(7);
        }

        private void button8_Click(object sender, EventArgs e)
        {
            addNum(8);
        }

        private void button9_Click(object sender, EventArgs e)
        {
            addNum(9);
        }

        private void button10_Click(object sender, EventArgs e)
        {
            addNum(0);
        }

        private void button13_Click(object sender, EventArgs e)
        {
            pos = 1;
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = "";
        }

        private void button14_Click(object sender, EventArgs e)
        {
            pos = 2;
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = "";
        }

        private void button15_Click(object sender, EventArgs e)
        {
            pos = 3;
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = "";
        }

        private void button16_Click(object sender, EventArgs e)
        {
            pos = 4;
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = "";
        }

        private void button12_Click(object sender, EventArgs e)
        {
            float number2 = Convert.ToInt64(textBox1.Text);
            switch (pos){
                case 1:
                    textBox1.Text = (number1 + number2).ToString();
                    break;
                case 2:
                    textBox1.Text = (number1 - number2).ToString();
                    break;
                case 3:
                    textBox1.Text = (number1 * number2).ToString();
                    break;
                case 4:
                    textBox1.Text = (number1 / number2).ToString();
                    break;
                case 5:
                    textBox1.Text = (Math.Pow(number1, number2)).ToString();
                    break;
                case 6:
                    textBox1.Text = (Math.Pow(number1, 1.0/number2)).ToString();
                    break;
            }
        }

        private void button17_Click(object sender, EventArgs e)
        {
            textBox1.Text = "";
            number1 = 0;
            pos = 0;
        }

        private void button18_Click(object sender, EventArgs e)
        {
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = (Math.Pow(number1, 2)).ToString();
            
        }

        private void button19_Click(object sender, EventArgs e)
        {
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = (Math.Pow(number1, 3)).ToString();
        }

        private void button20_Click(object sender, EventArgs e)
        {
            pos = 5;
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = "";
        }

        private void button21_Click(object sender, EventArgs e)
        {
            textBox1.Text =Math.PI.ToString();
        }

        private void button22_Click(object sender, EventArgs e)
        {
            Random random = new Random();
            int n = random.Next(1, 7);
            textBox1.Text = n.ToString();
        }

        private void button11_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + ".";
        }

        private void button23_Click(object sender, EventArgs e)
        {
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = (Math.Sqrt(number1)).ToString();
        }

        private void button24_Click(object sender, EventArgs e)
        {
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = (Math.Pow(number1, 1.0/3.0)).ToString();
        }

        private void button26_Click(object sender, EventArgs e)
        {
            textBox1.Text = Math.E.ToString();
        }

        private void button25_Click(object sender, EventArgs e)
        {
            pos = 6;
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = "";
        }
    }
}
