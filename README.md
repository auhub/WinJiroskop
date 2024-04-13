Jiroskop X, Y ve Z düzlemlerinde rotasyon belirlemede kullanılan ve genellikle uçak, insansı robot uygulamalarında bulunan bir araçtır. Jiroskop, üzerine sabitlendiği cismin yerçekimine göre ve Z eksenindeki rotasına göre anlamlı ve stabil değer üretir. Bu değeri işlemden geçirerek objenin rotasyonu ile ilgili her türden işlem yapabilirsiniz.

Bu projede Arduino sistemi ile bir MPU6050 6 eksenli ivme ve gyro sensörü (gy521) kullanarak fiziksel ortamdaki rotasyonun bilgisayardaki bir objeye doğrudan yansıtılmasını sağlayacağız. Projenin videosunu yazının sonunda bulabilirsiniz.

Projeyi taklit etmek isterseniz tüm adımları ve kodarı aşağıda veriyor olacağım.

Proje iki kattan oluşuyor. Birinci kat donanım katı yani Arduino ile sensörün okuduğu verileri anlamlı hale getirmemiz gerekiyor. İkinci katta ise arduinonun anlamlandırılmış verilerini işlememiz gerekiyor. Birinci katta C# ikinci katta VB dillerini kullanacağız.

Donanım Hazırlama

Sensörün SDA pinini Arduino’nun A4 (Analog 4) pinine, SCL pinini Arduino’nun A5 (Analog 5) pinine bağlayın.

Sensörü VCC girişinden Aruino’nın 3.3V çıkışı ile besleyin. Sensörün GND pinini Aruino’nun GND pinine topraklayın. Son olarak sensörün INT pinini Arduino’nun 2 numaralı dijital pinine bağlayın. Sistem çaıştığı sürece USB ile bilgisayara bağlı olmalıdır. Hata vb. durumlarda USB’den ayırmanızda herhangi bir sorun olmaz.
