# VORONOI-Zaman-Haritası-2026
Zamanı karelere hapsetmek yerine doğanın akışına bırakan; Voronoi tabanlı, kurulumsuz ve organik bir alışkanlık takip uygulaması.

Bu proje, "Zinciri Kırma" (Don't Break the Chain) üretkenlik metodolojisini temel alan, web tabanlı, interaktif ve açık kaynaklı bir alışkanlık takip uygulamasıdır. Standart kareli takvimlerin aksine, zamanı doğrusal olmayan ve organik bir yapıda görselleştirmek için **Voronoi diyagramları** kullanır.

## Felsefe

Geleneksel takvimler zamanı eşit, köşeli ve birbirinden kopuk karelere böler. Ancak hayat ve doğa doğrusal ilerlemez, daha akışkandır.

**Voronoi Diyagramı**, bir alanı en verimli, esnek ve sağlam şekilde bölmenin matematiksel karşılığıdır. Doğada zürafa desenlerinde, yaprak damarlarında veya çatlamış topraklarda görülen bu yapı, her parçanın komşusundan güç aldığı bir bütünü temsil eder.

Bu uygulamada günler:
1.  **Standart ızgaralar yerine organik hücrelerdir.** Her günün şekli biricik ve kendine hastır.
2.  **Yılan (Snake) dizilimi ile sıralanır.** Göz takibi soldan sağa, sonra bir alt satırda sağdan sola kıvrılarak ilerler; bu da zamanın kesintisiz akışını simgeler.
3.  **Fiziksel bağlar kurar.** "Zincir Modu" aktif edildiğinde, art arda tamamlanan günler arasında kırmızı bir bağ oluşur. Bu, soyut bir istikrarı somut bir ağa dönüştürür.

## Özellikler

* **Dinamik Voronoi Üretimi:** D3.js ve Lloyd's Relaxation algoritması kullanılarak her yenilemede matematiksel olarak dengeli ancak doğal görünümlü hücreler oluşturulur.
* **Veri Kalıcılığı (Persistence):** Tüm veriler (işaretlenen günler, hedefler, renk tanımları) tarayıcının `LocalStorage` alanında saklanır. Sayfa yenilense bile veri kaybolmaz.
* **Zincir Modu:** Arka arkaya gelen (n ve n+1) günler işaretlendiğinde, bu hücreler arasında otomatik olarak görsel bir bağlantı çizgisi çizilir.
* **Tıkla-Düzenle (Click-to-Edit):** Yıllık ve aylık hedefler, görüntüleme modunda sade bir metin, tıklandığında ise düzenlenebilir bir alan olarak çalışır.
* **Durum Takibi:** Her ay ve yıl geneli için "Oldu", "Kısmen", "Olmadı" şeklinde durum butonları bulunur.
* **Odak Modu:** "Hedefleri Göster" anahtarı kapatıldığında, tüm metin alanları gizlenerek sadece Voronoi haritasına odaklanılır.
* **Ekran Görüntüsü Alma:** Araç çubuğu hariç tüm takvimi yüksek çözünürlüklü PNG formatında dışa aktarma özelliği bulunur.

## Teknik Altyapı

Proje, harici bir backend veya veritabanı gerektirmeyen "Single Page Application" (SPA) mantığıyla tek bir HTML dosyası olarak çalışır.

* **Core:** HTML5, CSS3 (Grid/Flexbox), Vanilla JavaScript (ES6+)
* **Matematik & Grafik:** [D3.js](https://d3js.org/) (Delaunay üçgenlemesi ve Voronoi hesaplamaları için)
* **Görüntü İşleme:** [html2canvas](https://html2canvas.hertzen.com/) (DOM elementlerini Canvas'a render etmek için)
* **Font:** Google Fonts (Oswald)

## Kurulum ve Kullanım

Bu uygulama sunucu kurulumu gerektirmez.

1.  Kaynak kodu `index.html` adıyla kaydedin.
2.  Dosyayı herhangi bir modern web tarayıcısında (Chrome, Firefox, Edge, Safari) açın.
3.  Uygulama kullanıma hazırdır.

## Kullanım Kılavuzu

### 1. Hedef Belirleme
En üstteki alana 2026 yılı için ana hedefinizi girin. Her ayın altındaki alana ise o aya özel alt hedeflerinizi yazın. Metin alanlarına tıklayarak düzenleme moduna geçebilirsiniz.

### 2. Renk Paleti ve İşaretleme
Üst kısımdaki renk paletinden bir duygu veya durum seçin. Seçilen renk ile takvimdeki ilgili güne tıklayarak boyama yapın. Renklerin yanındaki etiketleri kendi sisteminize göre yeniden adlandırabilirsiniz.

### 3. Zincir Modu
Üst menüdeki "Zincir Modu" anahtarını açtığınızda, birbirini takip eden günlerde kopukluk yoksa hücreler arasında kırmızı bir bağlantı çizgisi belirir.

### 4. Kayıt ve Dışa Aktarma
Yaptığınız tüm değişiklikler anlık olarak tarayıcınıza kaydedilir. Yıl sonunda veya ay sonunda tablonuzu saklamak için "Resmi Kaydet" butonunu kullanabilirsiniz.

## Lisans

Bu proje açık kaynaklıdır, eğitim ve kişisel kullanım amacıyla özgürce geliştirilebilir ve dağıtılabilir.
