# Konu: Git ve GitHub

**GitHub Repo Adresim:** https://github.com/turgayenesgndz-stack/web-programciligi-3

 Araştırma

* **Git nedir?** Yazdığımız kodların geçmişini bilgisayarda adım adım kayıt altında tutan versiyon kontrol sistemidir.
* **GitHub nedir?** Git ile takip ettiğimiz projeleri internete yüklediğimiz, yedeklediğimiz ve başkalarıyla paylaştığımız web sitesidir.
* **Git ile GitHub arasındaki fark nedir?** Git bilgisayarımızda çalışan programdır (internetsiz de çalışır). GitHub ise bu kodları bulutta saklayan platformdur.
* **Repository nedir?** Projenin tüm dosya ve geçmiş kayıtlarının tutulduğu ana proje klasörüdür (kısaca repo denir).
* **Commit nedir?** Kodda yaptığımız değişiklikleri kısa bir açıklama yazarak kaydetme işlemidir. Oyunda "save almak" gibidir.
* **Branch nedir?** Ana çalışan kodu (`main`) bozmadan yeni bir özellik denemek için açtığımız yan çalışma dalıdır.
* **Merge nedir?** Yan dalda (branch) bitirdiğimiz kodu tekrar ana kodla birleştirme işlemidir.
* **Clone nedir?** GitHub'daki bir projeyi kendi bilgisayarımıza ilk defa indirmektir.
* **Pull nedir?** Projede başkalarının yaptığı son güncellemeleri kendi bilgisayarımıza çekmektir.
* **Push nedir?** Bilgisayarda aldığımız commit'leri (kayıtları) GitHub'a göndermektir.
* **.gitignore dosyasının amacı nedir?** GitHub'a yüklenmesini istemediğimiz gereksiz veya gizli dosyaları (şifreler, ayar dosyaları, büyük paket klasörleri) hariç tutmak için kullanılır.

**Hangi problemi çözer ve neden kullanılır?**
Projeyi geliştirirken klasörleri `proje_son`, `proje_enson_2` diye kopyalama derdini bitirir. Kod bozulduğunda çalışan eski haline tek tıkla dönmemizi sağlar. Ekipçe çalışırken herkesin birbirinin kodunu ezmeden aynı anda çalışmasına imkan verir.

**Avantajları, Dezavantajları ve Alternatifleri:**
* *Avantajları:* Kod kaybını önler, ekip çalışmasını kolaylaştırır, kim hangi satırı değiştirmiş görmemizi sağlar.
* *Dezavantajları:* İlk başta komutları ve kod çakışmalarını (conflict) çözmek biraz kafa karıştırıcıdır.
* *Alternatifleri:* GitHub yerine **GitLab** veya **Bitbucket**; Git yerine ise eski sistemlerden **SVN** kullanılabilir.

## Sektörde Kullanımı
Şirketlerde yazılımcılar ana koda (`main`) doğrudan kod atmaz. Herkes yapacağı iş için ayrı bir `branch` açar, işini bitirince **Pull Request (PR)** gönderir. Takım lideri kodu kontrol edip onayladıktan sonra ana projeye birleştirir (`merge`). Böylece canlıdaki web sitesi hiç çökmeden yeni özellikler eklenir.

## İncelediğim Projeler

GitHub üzerinden incelediğim 3 açık kaynak web projesi:

**1. Cal.com**
* **GitHub Adresi:** https://github.com/calcom/cal.com
* **Dil ve Framework:** TypeScript / Next.js, Tailwind CSS
* **Amacı:** Açık kaynaklı online randevu ve takvim yönetim uygulaması.
* **İstatistikler:** Yaklaşık 25.000+ commit ve 950+ katılımcı (contributor).
* **Klasör ve README Yapısı:** `apps` klasöründe web arayüzü, `packages` kısmında ortak modüller var. README dosyasında projenin ekran görüntüsü ve bilgisayarda çalıştırma komutları adım adım yazılmış.
* **Dikkatimi Çeken Nokta:** Çok fazla kişi çalışmasına rağmen herkesin commit mesajlarını standart ve kısa kurallarla yazması.

**2. Ghost**
* **GitHub Adresi:** https://github.com/TryGhost/Ghost
* **Dil ve Framework:** JavaScript / Node.js, Express
* **Amacı:** Blog ve haber siteleri için hızlı içerik yönetim sistemi (WordPress alternatifi).
* **İstatistikler:** Yaklaşık 45.000+ commit ve 600+ contributor.
* **Klasör ve README Yapısı:** Backend (`core`) ve yönetim paneli (`admin`) iki ayrı klasöre bölünmüş. README dosyası sade tutulmuş, kurulum linkleri net verilmiş.
* **Dikkatimi Çeken Nokta:** Yıllardır geliştirilen bir proje olduğu için sürüm geçmişinin çok düzenli tutulması.

**3. Excalidraw**
* **GitHub Adresi:** https://github.com/excalidraw/excalidraw
* **Dil ve Framework:** TypeScript / React
* **Amacı:** Tarayıcı üzerinden çalışan, el çizimi görünümünde diyagram ve beyaz tahta çizim aracı.
* **İstatistikler:** Yaklaşık 6.500+ commit ve 400+ contributor.
* **Klasör ve README Yapısı:** Kodlar doğrudan `src` (kaynak) klasörü altında bileşenlere ayrılmış. README'de canlı demo linki ve hızlı kurulum adımları var.
* **Dikkatimi Çeken Nokta:** Kurulumunun çok basit olması ve `.gitignore` dosyasının çok temiz hazırlanması.

## Yaptığım Uygulama
Bu dönem geliştireceğim **"Ne Var Ne Yok" (Malzemeye Göre Yemek Tarifi Sitesi)** projem için GitHub'da `web-programciligi-3` adında bir repository açtım. İçerisine projenin temel HTML dosyalarını, `.gitignore` dosyasını ve dokümantasyonu ekledim. Her adımı ayrı ve anlamlı commit mesajlarıyla kaydettim.

**Kurulum:**
1. Projeyi indirin: `git clone https://github.com/turgayenesgndz-stack/web-programciligi-3.git`
2. Klasöre girip `index.html` dosyasını tarayıcıda açın.

## Karşılaştığım Problemler
İlk başta commit mesajlarını neye göre yazacağımı bilemedim. Hoca yönergede `deneme`, `son` gibi isimler yasak dediği için açık kaynak projelere baktım ve her yaptığım değişikliği İngilizce kısa cümlelerle (`Add homepage`, `Add contact page` gibi) kaydettim.

## Öğrendiklerim
* Git ile GitHub'ın farkını ve kodları neden adım adım commit'lememiz gerektiğini öğrendim.
* `.gitignore` ile gereksiz dosyaları gizlemeyi ve standart bir `README.md` dosyası hazırlamayı öğrendim.

## Kaynaklar
* Git Resmi Sitesi: https://git-scm.com/doc
* GitHub Rehberi: https://docs.github.com/en/get-started
* İncelenen Repolar: Cal.com, Ghost ve Excalidraw GitHub sayfaları.
