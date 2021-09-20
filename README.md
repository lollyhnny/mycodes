# mycodes
ilk denemeler
//cafe içecek sipariş uygulaması :form uygulaması kullanarak masaüstü uygulaması tasarımı yaptım.(c#)


namespace CafeSiparis
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }




        private void caySayisiArttir_Click(object sender, EventArgs e)
        {
            int caySayisi = Convert.ToInt32(caySayisiLabel.Text);


            caySayisi++;
            caySayisiLabel.Text = Convert.ToString(caySayisi);


        }

        private void caySayisiAzalt_Click(object sender, EventArgs e)
        {
            int caySayisi = Convert.ToInt32(caySayisiLabel.Text);
            if (caySayisi > 0)
            {
                caySayisi--;
                caySayisiLabel.Text = Convert.ToString(caySayisi);
            }

        }

        private void kahveSayisiArttir_Click(object sender, EventArgs e)
        {
            int kahveSayisi = Convert.ToInt32(kahveSayisiLabel.Text);

            kahveSayisi++;
            kahveSayisiLabel.Text = Convert.ToString(kahveSayisi);


        }

        private void kahveSayisiAzalt_Click(object sender, EventArgs e)
        {
            int kahveSayisi = Convert.ToInt32(kahveSayisiLabel.Text);
            if (kahveSayisi > 0)
            {
                kahveSayisi--;
                kahveSayisiLabel.Text = Convert.ToString(kahveSayisi);
            }

        }

        private void limonataSayisiArttir_Click(object sender, EventArgs e)
        {
            int limonataSayisi = Convert.ToInt32(limonataSayisiLabel.Text);

            limonataSayisi++;
            limonataSayisiLabel.Text = Convert.ToString(limonataSayisi);


        }

        private void limonataSayisiAzalt_Click(object sender, EventArgs e)
        {
            int limonataSayisi = Convert.ToInt32(limonataSayisiLabel.Text);
            if (limonataSayisi > 0)
            { 
                limonataSayisi--;
                limonataSayisiLabel.Text = Convert.ToString(limonataSayisi);
            }

        }

        private void suSayisiArttir_Click(object sender, EventArgs e)
        {
            int suSayisi = Convert.ToInt32(suSayisiLabel.Text);

            suSayisi++;
            suSayisiLabel.Text = Convert.ToString(suSayisi);



        }

        private void suSayisiAzalt_Click(object sender, EventArgs e)
        {
            int suSayisi = Convert.ToInt32(suSayisiLabel.Text);
            if (suSayisi > 0)
            {
                suSayisi--;
                suSayisiLabel.Text = Convert.ToString(suSayisi);
            }

        }

        private void kolaSayisiArttir_Click(object sender, EventArgs e)
        {
            int kolaSayisi = Convert.ToInt32(kolaSayisiLabel.Text);

            kolaSayisi++;
            kolaSayisiLabel.Text = Convert.ToString(kolaSayisi);


        }

        private void kolaSayisiAzalt_Click(object sender, EventArgs e)
        {
            int kolaSayisi = Convert.ToInt32(kolaSayisiLabel.Text);
            if (kolaSayisi > 0)
            {
                kolaSayisi--;
                kolaSayisiLabel.Text = Convert.ToString(kolaSayisi);
            }

        }

        private void sifirlaButton_Click(object sender, EventArgs e)
        {
            caySayisiLabel.Text = "0";
            kahveSayisiLabel.Text = "0";
            limonataSayisiLabel.Text = "0";
            suSayisiLabel.Text = "0";
            kolaSayisiLabel.Text = "0";

        }

        private void tamamlaButton_Click(object sender, EventArgs e)
        {

            MessageBox.Show(caySayisiLabel.Text + " adet çay" + Environment.NewLine + kahveSayisiLabel.Text + " adet kahve" +
               Environment.NewLine + limonataSayisiLabel.Text + "  adet limonata  " + Environment.NewLine + suSayisiLabel.Text +
               " adet su" + Environment.NewLine + kolaSayisiLabel.Text + "  adet kola sipariş verdiniz.");
            
         

        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void buttonClose_Click(object sender, EventArgs e)
        {
            Close();
        }
    }
}
