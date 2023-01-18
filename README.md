# ParkourRace
<h3 align="center">22360859353 Berkan Serbes</h3>

<hr>
<p align="center">Oyunu tarayıcınızda oynamak için <a href="https://simmer.io/@berkanserbes/parkour-race" target="_blank"> tıklayın</a></p>
<hr>

# 3D 2 Kişilik Parkur Yarışı Oyunu 

## Oyunun Adı: Parkour Race 

## Oyunun Amacı
Parkurda bulunan iki oyuncunun kendi parkurunun bitiş noktasına rakibinden önce ulaşarak galip gelmek.

Bu proje vize projesinin devamı niteliğindedir. Vize projesini görüntülemek için <a href="https://github.com/berkanserbes/OyunProgramlama_VizeProjesi" target="_blank">tıklayın</a>.

## Oyun Tuşları

| **Oyuncu 1** | **Oyuncu 2** |      |
|-------------:|-------------|-------|
| **Tuş**      | **Tuş**     | **Görev** |
| W            |    ↑        | İleri hareket etme         |
| A            |    ←        | Sola hareket etme          |
| S            |    ↓        | Geriye hareket etme        |
| D            |    →        | Sağa hareket etme          |
| Space        |    Right Shift | Zıplama                 |
| Left Shift   |    AltGr        | Skill Kullanma         |

## Oyun İçi Mekanikler & Sahneler

### Ana menü ekranı

Oyun ilk açıldığında ana menü ekranı karşımıza çıkmaktadır. Bu ana menüde kullanıcı 'Yeni Oyun' butonuna tıklayarak oyunun ilk sahnesine geçiş yapabilir.
Kayıtlı bir oyunu varsa 'Devam Et' butonuna tıklayarak kaydedilmiş sahneden oyuna devam edebilir. 'Devam Et' butonu oyun ilk açıldığında pasif durumdadır.

![Ana Menu]()

Oyun ekranı, sol tarafta Player1'in kamerası ve sağ tarafta Player2'nin kamerası olmak üzere ikiye bölünmüştür. Ekranın üst orta kısmında kaçıncı bölümde olduğunu gösteren text ve sağ-sol üst kısımda oyuncuların skorlarını gösteren textler yer almaktadır. Her bir oyuncunun üstünde rakip oyuncuya skill uygulanabilirlik durumunu gösteren bir animasyon yer almaktadır, bu animasyon etkin olduğunda oyuncular birbirlerine skill (Zıplatma, Rastgele kuvvet uygulama) uygulayabilir.

![Dual Camera](https://github.com/berkanserbes/OyunProgramlama_VizeProjesi/blob/main/ScreenShot/DualCamera.png?raw=true)

### Atış bölümü

Bu kısımda oyuncular duvardaki hedefleri yok ederek oyuna devam ederler. Hedefler yeşil ve kırmızı olmak üzere iki renkten oluşur ve belirli aralıklarla renkleri değişir. Eğer hedefin rengi yeşilse Oyuncu1 klavyenin solunda bulunan Shift tuşuyla, Oyuncu2 ise AltGr tuşuyla hedefleri yok edebilir. Oyuncular bu hedefleri kırarken yerdeki lazerlerin üzerinden zıplamalıdırlar eğer lazerlerin üzerine basarlarsa en yakın spawn noktasından oyuna devam ederler.

![Target Area](https://github.com/berkanserbes/OyunProgramlama_VizeProjesi/blob/main/ScreenShot/ShootTarget.png?raw=true)

### Kutu bölümü

Bu kısımda oyuncular karşıdan gelen kutulardan kaçıp güvenli bölgelere ilerleyerek bu kısmı aşmak zorundadır. Eğer oyuncular kutu nesnesiyle çarpışırlarsa kutu tarafından platformun dışına sürüklenir.

![Box Collision](https://github.com/berkanserbes/OyunProgramlama_VizeProjesi/blob/main/ScreenShot/BoxCollision.png?raw=true)

### Spawn Noktaları

Oyun parkuru bölümlere ayrılmıştır ve bu bölümlerin her bir noktası bir spawn noktasıdır. Oyuncu parkurun dışına düştüğünde veya lazerin üzerine bastığında en yakın spawn noktasından oyuna devam eder.


### 2.Sahne

Oyunculardan herhangi biri birinci sahnenin bitiş noktasına ulaştığında ikinci sahneye geçiş yapılır. İkinci sahne birinci sahnenin aynısıdır.
İkinci oyun sahnesinde parkurun bitiş çizgisine ilk ulaşan oyuncu oyunu kazanır. Oyunun sonunda oyunu kazanan kişiyi gösteren ekran ortaya çıkar ve kullanıcı, ana menü ekranına yönlendirilir.
![Second Scene]()
![Winner Screen](https://github.com/berkanserbes/OyunProgramlama_VizeProjesi/blob/main/ScreenShot/WinnerScreen.png?raw=true)


Herhangi bir oyuncu ESC tuşuna bastığında oyun duraklatılır ve durdurma menüsü açılır. Bu durdurma menüsünde 'Devam Et', 'Yeniden Başlat' ve 'Ana Menü' adlı üç adet buton bulunmaktadır. Oyuncu 'Devam Et' butonuna basarak oyuna kaldığı yerden devam edebilir. 'Yeniden Başlat' butonuna basarak oyuna yeniden başlayabilir. 'Ana Menü' butonuna basarak Ana Menü ekranına geçiş yapabilir ya da yeniden ESC tuşuna basarak bu durdurma menüsünü kapatabilir.

![Pause Menu](https://github.com/berkanserbes/OyunProgramlama_VizeProjesi/blob/main/ScreenShot/PauseMenu.png?raw=true)

<hr>

## Oyunu Geliştirenler ve Görevleri

<h3>Samet Özkan</h3>

* Animasyon
* Ses ve Müzik
* Oynanabilir Sahneler

<h3>Berkan Serbes</h3>

* Ana Menü
* Kayıt Alma