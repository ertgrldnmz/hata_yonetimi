# Hata Yönetimi(Try-Catch-Finally)

```
try
    {
     Console.WriteLine("bir sayı giriniz:");
       int sayi=Convert.ToInt32(Console.ReadLine());
       Console.WriteLine("Girilen sayı:"+sayi);
       

       }
       catch(Exception ex)
       {
        Console.WriteLine("Hata:"+ex.Message.ToString());

       }
       finally
       {
        Console.WriteLine("işlem tamamlandı");

       }
      

       try
       {
            //int a=int.Parse(null);
            //int a=int.Parse("test");
            int a=int.Parse("-111111111111");
       }
       catch(ArgumentException  ex)
       {
        Console.WriteLine("Boş değer girdiniz");
        Console.WriteLine(ex);
       }
      
       catch(FormatException ex)
       {
        Console.WriteLine("veri tipi uygun değil");
        Console.WriteLine(ex);
       }
      
       catch(OverflowException ex)
       {
        Console.WriteLine("Girilen değer int veri aralığı arasında değil.");
        Console.WriteLine(ex);
       }
       
       finally
       {
        Console.WriteLine("işlem tamamlandı");

       }
    
      ```