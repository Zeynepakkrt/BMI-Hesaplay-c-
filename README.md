namespace BMII
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void Form1_Load(object sender, EventArgs e)
        {
            {
                comboBox1.Items.Add("pounds");
                comboBox1.Items.Add("stones");
                comboBox1.Items.Add("kilograms");
                comboBox2.Items.Add("inches");
                comboBox2.Items.Add("centimeters");
            }
        }

        private void button2_Click(object sender, EventArgs e)
        {
            foreach (Control c in this.Controls)
            {
                if (c is TextBox)
                {
                    TextBox tb = (TextBox)c;
                    tb.Clear();
                }
            }
        }

        private void button1_Click(object sender, EventArgs e)
        {
            double x, y, bmı;
            if (comboBox1.Text == "kilograms")
            {
                
                if (comboBox2.Text == "centimeters")
                {
                    y = Convert.ToDouble(textBox2.Text);
                    x = Convert.ToDouble(textBox1.Text) * Convert.ToDouble(textBox1.Text);
                    bmı = x / y;

                    if (bmı < 16.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Ağır derecede zayıf");
                    }
                    else if (bmı >= 16.0 && bmı < 18.4)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 18.5 && bmı < 24.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Normal");
                    }
                    else if (bmı >= 25.0 && bmı < 29.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 30.0 && bmı < 34.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Orta obez");
                    }
                    else if (bmı >= 35.0 && bmı < 39.8)
                    {
                        label3.Text = Convert.ToString(bmı + " Şiddetli obez");
                    }
                    else if (bmı >= 40.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Morbid obez");
                    }
                    

                }
                else if (comboBox2.Text == "inches")
                {
                    y = Convert.ToDouble(textBox2.Text);
                    x = Convert.ToDouble(textBox1.Text) * Convert.ToDouble(textBox1.Text);
                    bmı = x / y;

                    if (bmı < 16.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Ağır derecede zayıf");
                    }
                    else if (bmı >= 16.0 && bmı < 18.4)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 18.5 && bmı < 24.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Normal");
                    }
                    else if (bmı >= 25.0 && bmı < 29.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 30.0 && bmı < 34.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Orta obez");
                    }
                    else if (bmı >= 35.0 && bmı < 39.8)
                    {
                        label3.Text = Convert.ToString(bmı + " Şiddetli obez");
                    }
                    else if (bmı >= 40.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Morbid obez");
                    }
                    
                }

            }
            else if (comboBox1.Text == "stones")
            {
               
                if (comboBox2.Text == "centimeters")
                {
                    y = Convert.ToDouble(textBox2.Text) * Convert.ToDouble(textBox2.Text);
                    x = (703 * Convert.ToDouble(textBox1.Text));
                    bmı = x / y;

                    if (bmı < 16.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Ağır derecede zayıf");
                    }
                    else if (bmı >= 16.0 && bmı < 18.4)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 18.5 && bmı < 24.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Normal");
                    }
                    else if (bmı >= 25.0 && bmı < 29.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 30.0 && bmı < 34.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Orta obez");
                    }
                    else if (bmı >= 35.0 && bmı < 39.8)
                    {
                        label3.Text = Convert.ToString(bmı + " Şiddetli obez");
                    }
                    else if (bmı >= 40.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Orbid obez");
                    }
                    
                }
                else if (comboBox2.Text == "inches")
                {
                    y = Convert.ToDouble(textBox2.Text) * Convert.ToDouble(textBox2.Text);
                    x = (703 * Convert.ToDouble(textBox1.Text));
                    bmı = x / y;

                    if (bmı < 16.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Ağır derecede zayıf");
                    }
                    else if (bmı >= 16.0 && bmı < 18.4)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 18.5 && bmı < 24.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Normal");
                    }
                    else if (bmı >= 25.0 && bmı < 29.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 30.0 && bmı < 34.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Orta obez");
                    }
                    else if (bmı >= 35.0 && bmı < 39.8)
                    {
                        label3.Text = Convert.ToString(bmı + " Şiddetli obez");
                    }
                    else if (bmı >= 40.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Morbid obez");
                    }
                }
            }
            else if (comboBox1.Text == "pounds")
            {
               
                if (comboBox2.Text == "centimeters")
                {
                    y = Convert.ToDouble(textBox2.Text) * Convert.ToDouble(textBox2.Text);
                    x = (6.35 * Convert.ToDouble(textBox1.Text));
                    bmı = x / y;

                    if (bmı < 16.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Ağır derecede zayıf");
                    }
                    else if (bmı >= 16.0 && bmı < 18.4)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 18.5 && bmı < 24.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Normal");
                    }
                    else if (bmı >= 25.0 && bmı < 29.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 30.0 && bmı < 34.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Orta obez");
                    }
                    else if (bmı >= 35.0 && bmı < 39.8)
                    {
                        label3.Text = Convert.ToString(bmı + " Şiddetli obez");
                    }
                    else if (bmı >= 40.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Morbid obez");
                    }
                    
                }
                else if (comboBox2.Text == "inches")
                {
                    y = Convert.ToDouble(textBox2.Text) * Convert.ToDouble(textBox2.Text);
                    x = (6.35 * Convert.ToDouble(textBox1.Text));
                    bmı = x / y;

                    if (bmı < 16.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Ağır derecede zayıf");
                    }
                    else if (bmı >= 16.0 && bmı < 18.4)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 18.5 && bmı < 24.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Normal");
                    }
                    else if (bmı >= 25.0 && bmı < 29.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Kilolu");
                    }
                    else if (bmı >= 30.0 && bmı < 34.9)
                    {
                        label3.Text = Convert.ToString(bmı + " Orta obez");
                    }
                    else if (bmı >= 35.0 && bmı < 39.8)
                    {
                        label3.Text = Convert.ToString(bmı + " Şiddetli obez");
                    }
                    else if (bmı <= 40.0)
                    {
                        label3.Text = Convert.ToString(bmı + " Morbid obez");
                    }
                   
                }
            }                      
        }
    }
}
