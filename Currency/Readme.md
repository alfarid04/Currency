# Currency Apps

aplikasi ini mencakup fungsi perhitungan nilai tukar mata uang dari dollar ke rupiah.satu dolar dianggap Rp.15.000

# Scope&functionalities

-user dapat memasukan angka

-user dapat menyentuh tombol hitung

-user mendapat info "INVALID" jika yang dimasukan berupa text

# How does is works?

Diawali dengan method mainwindows pada class mainwindows.xaml.cs
code

``` java

       public MainWindow()
        {
            InitializeComponent();
            currency = new Currencycontroller();
        }
```
Logika perhitungan terdapat pada class currencycontroller.cs sebagai berikut

```java
     public string usdToIdr(string nominal)
        {
            var nominalDouble = Convert.ToDouble(nominal);
            var result = nominalDouble * 15000;
            return Convert.ToString(result);
        }
```