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
            double number2 = Convert.ToDouble(textBox1.Text);
            switch (pos)
            {
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
                    textBox1.Text = (Math.Pow(number1, 1.0 / number2)).ToString();
                    break;
                case 7:
                    textBox1.Text = (Math.Log(number1, number2)).ToString();
                    break;
            }
        }

        private void button17_Click(object sender, EventArgs e)
        {
            textBox1.Text = "";
            number1 = 0;
            pos = 0;
            textBox1.BackColor = Color.FromArgb(255, 255, 255);
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
            textBox1.Text = Math.PI.ToString();
        }

        private void button22_Click(object sender, EventArgs e)
        {
            Random random = new Random();
            int n = random.Next(1, 7);
            textBox1.Text = n.ToString();
            switch (n)
            {
                case 6:
                    textBox1.BackColor = Color.FromArgb(255, 23, 140);
                    textBox1.Text = textBox1.Text + "Congratulation";
                    break;
                case 1:
                    textBox1.BackColor = Color.FromArgb(192, 255, 192);
                    textBox1.Text = textBox1.Text + "What a pity";
                    break;
                case 2:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 5:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 4:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 3:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
            }

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
            textBox1.Text = (Math.Pow(number1, 1.0 / 3.0)).ToString();
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

        private void button27_Click(object sender, EventArgs e)
        {
            pos = 7;
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = "";
        }

        private void button28_Click(object sender, EventArgs e)
        {
            number1 = Convert.ToDouble(textBox1.Text);
            textBox1.Text = (Math.Log(Math.E, number1)).ToString();
        }

        private void Thereediceroll_Click(object sender, EventArgs e)
        {
            Random random = new Random();
            int n = random.Next(3, 19);
            textBox1.Text = n.ToString();
            switch (n)
            {
                case 18:
                    textBox1.BackColor = Color.FromArgb(255, 23, 140);
                    textBox1.Text = textBox1.Text + "Amazing";
                    break;
                case 3:
                    textBox1.BackColor = Color.FromArgb(192, 255, 192);
                    textBox1.Text = textBox1.Text + "What a pity";
                    break;
                case 6:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 5:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 4:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 7:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 8:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 9:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 10:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 11:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 12:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 13:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 14:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 15:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 16:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
                case 17:
                    textBox1.BackColor = Color.FromArgb(255, 255, 255);
                    break;
            }
        }

        private void button29_Click(object sender, EventArgs e)
        {
            Form2 nf = new Form2();
            nf.ShowDialog();

        }
    }
}
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
    public partial class Form2 : Form
    {
        double number1, number2, number3, number4;
        int pos;

        private void button2_Click(object sender, EventArgs e)
        {
            addNum(2);
        }

        private void button3_Click(object sender, EventArgs e)
        {
            addNum(3);
        }

        private void button4_Click(object sender, EventArgs e)
        {
            addNum(4);
        }

        private void button5_Click(object sender, EventArgs e)
        {
            addNum(5);
        }

        private void button6_Click(object sender, EventArgs e)
        {
            addNum(6);
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

        private void button11_Click(object sender, EventArgs e)
        {
            textBox1.Text = textBox1.Text + ".";
        }

        private void button12_Click(object sender, EventArgs e)
        {
            textBox1.Text = "输入提示的数值:";
            textBox2.Text = "";
            number1 = 0;
            number2 = 0;
            pos = 0;
            textBox1.BackColor = Color.FromArgb(255, 255, 255);
        }

        private void button13_Click(object sender, EventArgs e)
        {
            textBox1.Text = "Profit before interest and tax:";
            pos = 1;
            this.button14.Visible = true;
            this.button15.Visible = false;
            this.button16.Visible = false;
            this.button17.Visible = false;
        }

        private void button14_Click(object sender, EventArgs e)
        {
            number1 = Convert.ToDouble(textBox2.Text);
            switch (pos)
            {
                case (1):
                    textBox1.Text = "Total assets:";
                    this.button14.Visible = false;
                    this.button15.Visible = true;
                    textBox2.Text = "";
                    break;
                case (2):
                    textBox1.Text = "term debet:";
                    this.button14.Visible = false;
                    this.button15.Visible = true;
                    textBox2.Text = "";
                    break;
                case (3):
                    textBox1.Text = "Cn:";
                    this.button14.Visible = false;
                    this.button15.Visible = true;
                    textBox2.Text = "";
                    break;
            }
        }

        private void button15_Click(object sender, EventArgs e)
        {
            number2 = Convert.ToDouble(textBox2.Text);
            switch (pos)
            {
                case (1):
                    textBox1.Text = "current liabilities:";
                    this.button15.Visible = false;
                    this.button16.Visible = true;
                    textBox2.Text = "";
                    break;
                case (2):
                    textBox1.Text = "shareholders' equity:";
                    this.button15.Visible = false;
                    this.button16.Visible = true;
                    textBox2.Text = "";
                    break;
                case (3):
                    textBox1.Text = "ZOQ:";
                    textBox2.Text = Convert.ToString(Math.Sqrt((number1*2) / number2));
                    break;
            }
        }

        private void button16_Click(object sender, EventArgs e)
        {
            number3 = Convert.ToDouble(textBox2.Text);
            switch (pos)
            {
                case (1):
                    textBox1.Text = "Return on capital employed:";
                    textBox2.Text = Convert.ToString(number1 / (number2 - number3));
                    break;
                case (2):
                    textBox1.Text = "total long-term debt";
                    this.button16.Visible = false;
                    this.button17.Visible = true;
                    textBox2.Text = "";
                    break;

            }
        }

        private void button17_Click(object sender, EventArgs e)
        {
            number4 = Convert.ToDouble(textBox2.Text);
            switch (pos)
            { 
                case (2):
                    textBox1.Text = "Gearing:";
                    textBox2.Text = Convert.ToString((number1-number2) / (number3 + number4));
                    break;
            }
        }

        private void button18_Click(object sender, EventArgs e)
        {
            textBox1.Text = "Total lony:";
            pos = 2;
            this.button14.Visible = true;
            this.button15.Visible = false;
            this.button16.Visible = false;
            this.button17.Visible = false;
        }

        private void button19_Click(object sender, EventArgs e)
        {
            textBox1.Text = "C0D:";
            pos = 3;
            this.button14.Visible = true;
            this.button15.Visible = false;
            this.button16.Visible = false;
            this.button17.Visible = false;
        }

        public void addNum(int num)
        {
            textBox2.Text = textBox2.Text + num.ToString();

        }
        public Form2()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            addNum(1);
        }
    }
}
