# Constructor

namespace kurucumetodlar
{
    class program
    {
        static void Main(string[] args)
        {
            calisan calisan1=new calisan();
            calisan1.Ad="melike";
            calisan1.Soyad="tutkun";
            calisan1.No=123;
            calisan1.Departman="ik";
            calisan1.CaslisanBilgileri();

            calisan calisan2=new calisan("ayşe", "tutkun",20,"ik");
            calisan calisan3=new calisan("ayşe", "tutkun");
        }
        class calisan
        {
            public string Ad;
            public string Soyad;
            public int No;
            public string Departman;
            public calisan(string ad,string soyad,int no,string Departman)
            {
                this.Ad=ad;
                this.Soyad=soyad;
                this.No=no;
                this.Departman=Departman;
            }

            public calisan(string ad,string soyad)
            {
                this.Ad=ad;
                this.Soyad=soyad;
            }
            public calisan(){}
            public void CaslisanBilgileri()
            {
                Console.WriteLine("Çalışan Adı:{}",Ad);
                Console.WriteLine("Çalışan SoyAdı:{}",Soyad);
                Console.WriteLine("Çalışan No:{}",No);
                Console.WriteLine("Çalışan Departman:{}",Departman);
            }
        }

    }
}
