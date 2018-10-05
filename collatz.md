---
layout: default
---

## 콜라츠 알고리즘

```#
﻿using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApp1
{
    public partial class Form1 : Form
    {

        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            textBox2.Text = textBox1.Text;

            int input = int.Parse(textBox1.Text);
            int temp = input;

            List<int> tempList = new List<int>();

            chart1.Series["Series1"].Points.Clear();

            if (radioButton1.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else
                    {
                        temp = temp * 3 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp)==true)
                    {
                        break;
                    }
                    tempList.Add(temp);

                }
            }
            if (radioButton2.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else
                    {
                        temp = temp * 5 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
            if (radioButton3.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else if (temp % 5 == 0)
                    {
                        temp = temp / 5;
                    }
                    else
                    {
                        temp = temp * 7 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
            if (radioButton4.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else if (temp % 5 == 0)
                    {
                        temp = temp / 5;
                    }
                    else if (temp % 7 == 0)
                    {
                        temp = temp / 7;
                    }
                    else
                    {
                        temp = temp * 11 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
            if (radioButton5.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else if (temp % 5 == 0)
                    {
                        temp = temp / 5;
                    }
                    else if (temp % 7 == 0)
                    {
                        temp = temp / 7;
                    }
                    else if (temp % 11 == 0)
                    {
                        temp = temp / 11;
                    }
                    else
                    {
                        temp = temp * 13 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
            if (radioButton6.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else if (temp % 5 == 0)
                    {
                        temp = temp / 5;
                    }
                    else if (temp % 7 == 0)
                    {
                        temp = temp / 7;
                    }
                    else if (temp % 11 == 0)
                    {
                        temp = temp / 11;
                    }
                    else if (temp % 13 == 0)
                    {
                        temp = temp / 13;
                    }
                    else
                    {
                        temp = temp * 17 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
            if (radioButton7.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else if (temp % 5 == 0)
                    {
                        temp = temp / 5;
                    }
                    else if (temp % 7 == 0)
                    {
                        temp = temp / 7;
                    }
                    else if (temp % 11 == 0)
                    {
                        temp = temp / 11;
                    }
                    else if (temp % 13 == 0)
                    {
                        temp = temp / 13;
                    }
                    else if (temp % 17 == 0)
                    {
                        temp = temp / 17;
                    }
                    else
                    {
                        temp = temp * 19 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
            if (radioButton8.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else if (temp % 5 == 0)
                    {
                        temp = temp / 5;
                    }
                    else if (temp % 7 == 0)
                    {
                        temp = temp / 7;
                    }
                    else if (temp % 11 == 0)
                    {
                        temp = temp / 11;
                    }
                    else if (temp % 13 == 0)
                    {
                        temp = temp / 13;
                    }
                    else if (temp % 17 == 0)
                    {
                        temp = temp / 17;
                    }
                    else if (temp % 19 == 0)
                    {
                        temp = temp / 19;
                    }
                    else
                    {
                        temp = temp * 23 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
            if (radioButton9.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else if (temp % 5 == 0)
                    {
                        temp = temp / 5;
                    }
                    else if (temp % 7 == 0)
                    {
                        temp = temp / 7;
                    }
                    else if (temp % 11 == 0)
                    {
                        temp = temp / 11;
                    }
                    else if (temp % 13 == 0)
                    {
                        temp = temp / 13;
                    }
                    else if (temp % 17 == 0)
                    {
                        temp = temp / 17;
                    }
                    else if (temp % 19 == 0)
                    {
                        temp = temp / 19;
                    }
                    else if (temp % 23 == 0)
                    {
                        temp = temp / 23;
                    }
                    else
                    {
                        temp = temp * 29 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
            if (radioButton10.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else if (temp % 5 == 0)
                    {
                        temp = temp / 5;
                    }
                    else if (temp % 7 == 0)
                    {
                        temp = temp / 7;
                    }
                    else if (temp % 11 == 0)
                    {
                        temp = temp / 11;
                    }
                    else if (temp % 13 == 0)
                    {
                        temp = temp / 13;
                    }
                    else if (temp % 17 == 0)
                    {
                        temp = temp / 17;
                    }
                    else if (temp % 19 == 0)
                    {
                        temp = temp / 19;
                    }
                    else if (temp % 23 == 0)
                    {
                        temp = temp / 23;
                    }
                    else if (temp % 29 == 0)
                    {
                        temp = temp / 29;
                    }
                    else
                    {
                        temp = temp * 31 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
            if (radioButton11.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else if (temp % 5 == 0)
                    {
                        temp = temp / 5;
                    }
                    else if (temp % 7 == 0)
                    {
                        temp = temp / 7;
                    }
                    else if (temp % 11 == 0)
                    {
                        temp = temp / 11;
                    }
                    else if (temp % 13 == 0)
                    {
                        temp = temp / 13;
                    }
                    else if (temp % 17 == 0)
                    {
                        temp = temp / 17;
                    }
                    else if (temp % 19 == 0)
                    {
                        temp = temp / 19;
                    }
                    else if (temp % 23 == 0)
                    {
                        temp = temp / 23;
                    }
                    else if (temp % 29 == 0)
                    {
                        temp = temp / 29;
                    }
                    else if (temp % 31 == 0)
                    {
                        temp = temp / 31;
                    }
                    else
                    {
                        temp = temp * 37 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
            if (radioButton12.Checked == true)
            {
                while (temp > 1)
                {
                    chart1.Series["Series1"].Points.Add(temp);
                    if (temp % 2 == 0)
                    {
                        temp = temp / 2;
                    }
                    else if (temp % 3 == 0)
                    {
                        temp = temp / 3;
                    }
                    else if (temp % 5 == 0)
                    {
                        temp = temp / 5;
                    }
                    else if (temp % 7 == 0)
                    {
                        temp = temp / 7;
                    }
                    else if (temp % 11 == 0)
                    {
                        temp = temp / 11;
                    }
                    else if (temp % 13 == 0)
                    {
                        temp = temp / 13;
                    }
                    else if (temp % 17 == 0)
                    {
                        temp = temp / 17;
                    }
                    else if (temp % 19 == 0)
                    {
                        temp = temp / 19;
                    }
                    else if (temp % 23 == 0)
                    {
                        temp = temp / 23;
                    }
                    else if (temp % 29 == 0)
                    {
                        temp = temp / 29;
                    }
                    else if (temp % 31 == 0)
                    {
                        temp = temp / 31;
                    }
                    else if (temp % 37 == 0)
                    {
                        temp = temp / 37;
                    }
                    else
                    {
                        temp = temp * 41 + 1;
                    }
                    textBox2.Text = textBox2.Text + "," + temp;
                    if (tempList.Contains(temp) == true)
                    {
                        break;
                    }
                    tempList.Add(temp);
                }
            }
        }
    }
}
```

[back](./)
