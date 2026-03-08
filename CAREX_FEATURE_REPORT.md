# Carex Tema Özellik Raporu

## Yönetici Özeti

Carex zaten güçlü bir temele sahip: üç varyant, geniş UI kapsamı ve Catppuccin’e yakın ama daha derli toplu bir görsel kimlik. Bir sonraki büyüme adımı sadece daha fazla renk eklemek değil; Carex’i daha karakterli bir tema ailesine dönüştürmek, erişilebilirliği güçlendirmek, dil bazlı token kapsamını artırmak ve daha net bir sürüm stratejisi oluşturmaktır.

En yüksek değer üretecek yönler şunlardır:

1. Tema ailesini bilinçli biçimde ayrışan yeni varyantlarla genişletmek.
2. Semantic highlighting ve framework odaklı token ayarlarını iyileştirmek.
3. Dokümantasyon, önizlemeler ve isteğe bağlı tamamlayıcı varlıklarla marketplace tarafında daha fazla ayrışmak.
4. Erişilebilirliği tek bir high-contrast seçeneği yerine ayrı bir ürün hattı gibi ele almak.

## Mevcut Durum

Carex’in mevcut güçlü yönleri:

1. Dark, Light ve High Contrast varyantları temel kullanım senaryolarını zaten kapsıyor.
2. Renk paleti tanıdık ve konforlu olduğu için benimsenme eşiğini düşürüyor.
3. Eklenti, kod tabanlı aktivasyon yükü yerine tema odaklı olduğu için hafif kalıyor.
4. README sunumu marketplace dönüşümü için şimdiden yeterince güçlü.

Ele alınmaya değer mevcut boşluklar:

1. Sadece üç varyant olması, farklı kullanıcı zevkleri için sınırlı segmentasyon yaratıyor.
2. Ürün kimliği Catppuccin esintili temalara yakın; bu yüzden ayrışma daha da güçlendirilebilir.
3. Tema değeri genel şekilde anlatılıyor, ancak henüz özellik hatları veya yol haritası katmanlarına ayrılmış değil.
4. Erişilebilirlik tek bir high-contrast ön ayarın ötesine geçebilir.
5. Dil bazlı ince ayarlar Rust, Go, Java, PHP, C#, Astro, Svelte ve Tailwind ağırlıklı işaretleme gibi modern yığınlar için genişletilebilir.

## Önerilen Özellik Alanları

## 1. Yeni Tema Varyantları

Bunlar en görünür geliştirmelerdir çünkü kullanıcılar yeni varyantları anında fark eder.

### A. Carex OLED

Amaç:
OLED ekranlı dizüstüler ve maksimum kontrastı, daha az ekran parıltısıyla tercih eden kullanıcılar için saf siyah arka plan sunmak.

Önerilen yön:

1. Arka planı #000000 veya #050505 civarında tutmak.
2. Tamamen monokrom yapmak yerine Carex vurgu renklerini korumak.
3. Mevcut dark temaya göre biraz daha parlak imleç ve seçim renkleri kullanmak.
4. Siyah zeminler için ayarlanmış güçlü bir terminal ANSI paleti eklemek.

Neden önemli:
Bu, VS Code tema kategorisinde sık talep edilen bir alan ve pazarlaması kolaydır.

### B. Carex Dusk

Amaç:
Mevcut ana dark temadan daha sıcak ve daha atmosferik bir karanlık varyant sunmak.

Önerilen yön:

1. Arka planda arduvaz-mürdüm alt tonları kullanmak.
2. Mavi ağırlığını azaltıp mat mercan ve altın tonlarını artırmak.
3. Uzun okuma oturumları için daha yumuşak yorum renkleri ve daha düşük doygunluk kullanmak.

Neden önemli:
Carex kimliğini korurken daha editoryal, daha karakterli ve daha az “standart dark theme” hissi verir.

### C. Carex Dawn

Amaç:
Parlak light temaları yorucu bulan kullanıcılar için daha yumuşak bir açık tema sunmak.

Önerilen yön:

1. Çok parlak yüzeyler yerine sıcak, kağıt hissi veren kırık beyaz tonlara geçmek.
2. Kırmızı ve mavi tokenlarda doygunluk sıçramalarını azaltmak.
3. Kenarlık ve panel ayrımlarını göz kamaşmasını azaltacak şekilde ayarlamak.

Neden önemli:
Birçok kullanıcı light theme istiyor ama sert arka planlar nedeniyle kullanmıyor.

### D. Carex Neon

Amaç:
Daha çarpıcı vurgu renklerine sahip, gösterişli bir vitrin varyantı üretmek.

Önerilen yön:

1. Derin lacivert veya kömür tonlu bir taban kullanmak.
2. Elektrik cyan, mercan, lime ve magenta odaklı bir vurgu sistemi oluşturmak.
3. Güçlü bracket pair renklendirmesi ve daha cesur bir terminal paleti eklemek.

Neden önemli:
Sosyal medya paylaşımları, ekran görüntüleri ve marka ayrışması için güçlü bir seçenek olur.

### E. Erişilebilirlik Odaklı Varyantlar

Amaç:
Tek bir genel fallback yerine hedefe yönelik erişilebilirlik temaları sunmak.

Önerilen seçenekler:

1. Carex High Contrast Dark.
2. Carex High Contrast Light.
3. Carex Deuteranopia Friendly.
4. Carex Protanopia Friendly.
5. Carex Low Distraction.

Neden önemli:
Erişilebilirlik, yalnızca bir uyumluluk maddesi değil; somut bir ürün yüzeyi haline gelir.

## 2. Semantic Highlighting Genişletmesi

Tema kalitesinin gerçekten premium hissettirdiği alan burasıdır.

Öncelikli iyileştirmeler:

1. Sınıflar, enum’lar, interface’ler, type parameter’lar, decorator’lar ve readonly özellikler için semantic token renklerini iyileştirmek.
2. Fonksiyon tanımları ile fonksiyon çağrılarını görsel olarak ayrıştırmak.
3. Değiştirilebilir değişkenler ile sabitleri ayırt etmek.
4. Async anahtar sözcükler, operatörler, escape sequence’ler, regex grupları ve template literal’larda daha net token görünürlüğü sağlamak.
5. Yorumlar, doc comment’ler, TODO/FIXME işaretleri ve deprecated semboller için daha iyi görsel ayrım sunmak.

Önceliklendirilecek dil hedefleri:

1. TypeScript ve TSX.
2. JavaScript ve JSX.
3. Python.
4. JSON ve YAML.
5. Markdown.
6. CSS, SCSS ve Tailwind ağırlıklı HTML.
7. Rust.
8. Go.
9. Java.
10. C#.
11. PHP.
12. Svelte, Vue ve Astro.

Beklenen etki:
Kullanıcılar özellikle büyük kod tabanlarında temayı daha “akıllı” ve daha bilinçli tasarlanmış olarak algılar.

## 3. UI Kapsamı İyileştirmeleri

İyileştirilebilecek potansiyel workbench alanları:

1. Command palette durumları.
2. Quick input hover ve focus katmanları.
3. Sticky scroll arka planları ve kenarlıkları.
4. Modern VS Code sürümlerindeki inline chat veya AI ile ilgili UI elemanları.
5. Test explorer için başarılı, başarısız ve atlanan durum renkleri.
6. Git dekorasyonları: eklenen, değiştirilen, silinen, ignore edilen ve çakışmalı dosyalar.
7. Notebook hücreleri, çalıştırma durumu ve çıktı kenarlıkları.
8. Merge editor renkleri.
9. Peek view ve inline diff bileşenleri.
10. Editör paletiyle daha uyumlu terminal ANSI renkleri.

Neden önemli:
Editör renkleri iyi olsa bile yardımcı araçlar varsayılan görünüyorsa tema tamamlanmamış hissi verir.

## 4. Markdown ve Dokümantasyon Yazım Deneyimi

Bu alan güçlü bir niş fırsattır çünkü birçok geliştirici kod yazdığı kadar dokümantasyon da yazar.

Fikirler:

1. Başlıklar, alıntılar, inline code, listeler ve bağlantılar için daha iyi renk işleme.
2. Kod bloklarının sınırlarını ve alıntı arka planlarını daha okunur hale getirmek.
3. Markdown dosyalarındaki frontmatter için belirgin bir görsel stil oluşturmak.
4. Kalın, italik ve üstü çizili vurgular için daha net ayrım sağlamak.

Neden önemli:
Hem ekran görüntülerini iyileştirir hem de repo ağırlıklı iş akışlarında günlük kullanımı güçlendirir.

## 5. Framework’e Özel Tema İnce Ayarları

Carex’in genel amaçlı bir temadan akılda kalıcı bir ürüne dönüşebileceği alan burasıdır.

### Frontend yığınları

1. React ve JSX prop renklendirmesi.
2. Vue directive ve template expression görünürlüğü.
3. Svelte sözdizimi bölgeleri.
4. Astro component frontmatter ve island sözdizimi.
5. Tailwind class string’leri içinde utility token okunabilirliği.

### Backend ve sistem yığınları

1. Rust lifetime’ları, macro’ları, trait’leri ve mutable binding’leri.
2. Go interface’leri, receiver yapıları ve package adları.
3. Java annotation’ları, generics yapıları ve static üyeleri.
4. C# attribute’ları, record yapıları ve LINQ sözdizimi.
5. PHP anahtar sözcükleri, değişkenler ve heredoc/nowdoc kullanımları.

Neden önemli:
Framework uyumu, organik tavsiye edilme ve benimsenme oranını artırır.

## 6. Renk Temalarının Ötesindeki Tamamlayıcı Eklemeler

Bunlar zorunlu değil, ancak eklentiyi yalnızca bir tema paketinden daha güçlü bir marka ekosistemine dönüştürebilir.

Olası eklemeler:

1. Özel file icon theme.
2. Product icon theme.
3. Her varyant için dokümantasyonda önerilen ayar profilleri.
4. Her varyanta uyarlanmış bracket pair ön ayarları.
5. Popüler shell’ler ve terminal emülatörleri için isteğe bağlı terminal paleti çıktıları.
6. Sürüm duyuruları için duvar kağıdı veya sosyal medya önizleme varlıkları.

Önemli not:
Bu eklemeler VS Code eklenti ekosisteminde yapılabilir, ancak kapsamı büyütür; bu yüzden temel tema kalitesi çalışmaları tamamlandıktan sonra aşamalı ilerlemelidir.

## 7. Erişilebilirlik İyileştirmeleri

Erişilebilirlik açık biçimde tasarım çalışmasının bir parçası haline gelmelidir.

Önerilen yönler:

1. Yorumlar, satır numaraları, kılavuz çizgileri ve pasif UI durumları için minimum kontrast gözden geçirmesi.
2. Editör ve workbench genelinde hata, uyarı, bilgi ve başarı semantiğinin daha tutarlı hale getirilmesi.
3. Anlam iletmek için yalnızca renge bağımlılığın azaltılması.
4. Klavye ile gezinme için daha güçlü focus ring’ler.
5. Pasif seçim ve hover durumlarının daha görünür hale getirilmesi.
6. Daha yumuşatılmış dekorasyonlara sahip isteğe bağlı bir low-distraction modu.

Doğrulama yöntemleri:

1. Uygun yerlerde WCAG hedeflerine göre kontrast kontrolü yapmak.
2. Düşük ekran parlaklığı ve aydınlık ortam senaryolarında gerçek ekran görüntüleriyle test etmek.
3. Kırmızı-yeşil renk körlüğü simülatörleriyle manuel inceleme yapmak.

## 8. Marketplace ve Sunum Özellikleri

Bunlar, tema JSON karmaşıklığını çok artırmadan benimsenmeyi güçlendirir.

Önerilen iyileştirmeler:

1. README içinde varyant karşılaştırma tablosu.
2. Her varyant ve dil ailesi için özel önizleme ekran görüntüleri.
3. Gece kodlama, gündüz kullanımı, OLED, erişilebilirlik ve dokümantasyon gibi “best for” etiketleri.
4. Changelog maddelerini yalnızca ham değişikliklerle değil, kullanıcı faydasıyla çerçevelemek.
5. Yol haritası formatında görünür bir sürüm ritmi sunmak.
6. Net destek ve sponsorluk konumlandırması yapmak.

Neden önemli:
Marketplace görsel bir alandır; iyi konumlandırma kurulum sayısını anlamlı biçimde etkileyebilir.

## 9. Kalite ve Bakım İyileştirmeleri

Önerilen operasyonel iyileştirmeler:

1. Her sürüm öncesi bir token gözden geçirme kontrol listesi oluşturmak.
2. JS, TS, Python, Markdown, JSON, CSS, Rust ve Java için sabit ekran görüntüsü fixture’ları tutmak.
3. Temaları birden fazla VS Code sürümünde doğrulamak.
4. Yayınlamadan önce renk regresyonlarını yan yana karşılaştırmak.
5. Semver’i bilinçli kullanmak: renk düzeltmeleri için patch, yeni varyantlar için minor, büyük görsel resetler için major.

## Önerilen Sürüm Yol Haritası

## Faz 1: Hızlı Kazanımlar

Hedef: bir sonraki patch veya minor sürüm.

1. Sponsorluk/destek çağrısını README’nin en üstüne taşımak.
2. Yol haritası veya özellik raporu dosyası eklemek.
3. README varyant karşılaştırmasını iyileştirmek.
4. TypeScript, Python ve Markdown için semantic token ayarlarını güçlendirmek.
5. Terminal ANSI paleti tutarlılığını iyileştirmek.

## Faz 2: Ayrışma Sürümü

Hedef: bir sonraki minor sürüm.

1. Carex OLED eklemek.
2. Carex Dawn veya Carex Dusk eklemek.
3. React, Vue, Svelte ve Astro için framework’e özel token renklerini iyileştirmek.
4. Düşük kontrastlı UI durumları için erişilebilirlik incelemesini genişletmek.
5. Tüm varyantlar için güncel ekran görüntüleri yayınlamak.

## Faz 3: Ekosistem Sürümü

Hedef: daha büyük bir minor veya major sürüm.

1. Bir file icon theme veya product icon theme eklemek.
2. Erişilebilirliğe özel varyantlar sunmak.
3. Varyant bazlı önerilen ayar profilleri yayınlamak.
4. Marketplace görselleri ve dokümantasyon genelinde daha güçlü bir Carex marka sistemi oluşturmak.

## En Yüksek Öncelikli Öneriler

Eforun dar tutulması gerekiyorsa en iyi yatırım alanları şunlardır:

1. Carex OLED eklemek.
2. Daha yumuşak alternatif bir varyant eklemek: Carex Dawn veya Carex Dusk.
3. TS, Python, Markdown ve CSS için semantic token kapsamını genişletmek.
4. Terminal ve Git dekorasyonu uyumunu iyileştirmek.
5. Zaman içinde erişilebilirlik odaklı varyantlar eklemek.

## Önerilen İsim Genişlemeleri

Tema ailesini tutarlı korumak için kısa ve akılda kalıcı isimler kullanılabilir:

1. Carex Dark
2. Carex Light
3. Carex High Contrast
4. Carex OLED
5. Carex Dusk
6. Carex Dawn
7. Carex Neon
8. Carex Low Distraction

## Nihai Öneri

Carex, küçük ama premium bir tema ailesi olarak konumlanmalı; yalnızca ufak alternatifler içeren tek bir tema paketi gibi görünmemelidir. En doğru yol, yeni bir amiral gemisi varyantı, daha güçlü semantic token kalitesi ve görünür bir erişilebilirlik stratejisini bir araya getirerek sonraki sürümlerin daha bilinçli ve daha kolay pazarlanabilir olmasını sağlamaktır.