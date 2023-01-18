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

![Ana Menu](https://github.com/berkanserbes/OyunProgramlama_FinalProjesi/blob/main/ScreenShots/MainMenu.png?raw=true)

Oyun ekranı, sol tarafta Player1'in kamerası ve sağ tarafta Player2'nin kamerası olmak üzere ikiye bölünmüştür. Ekranın üst orta kısmında kaçıncı bölümde olduğunu gösteren text ve sağ-sol üst kısımda oyuncuların skorlarını gösteren textler yer almaktadır. Her bir oyuncunun üstünde rakip oyuncuya skill uygulanabilirlik durumunu gösteren bir animasyon yer almaktadır, bu animasyon etkin olduğunda oyuncular birbirlerine skill (Zıplatma, Rastgele kuvvet uygulama) uygulayabilir.

![Dual Camera](https://github.com/berkanserbes/OyunProgramlama_FinalProjesi/blob/main/ScreenShots/sahne1.png?raw=true)

### Atış bölümü

Bu kısımda oyuncular duvardaki hedefleri yok ederek oyuna devam ederler. Hedefler yeşil ve kırmızı olmak üzere iki renkten oluşur ve belirli aralıklarla renkleri değişir. Eğer hedefin rengi yeşilse Oyuncu1 klavyenin solunda bulunan Shift tuşuyla, Oyuncu2 ise AltGr tuşuyla hedefleri yok edebilir. Oyuncular bu hedefleri kırarken yerdeki lazerlerin üzerinden zıplamalıdırlar eğer lazerlerin üzerine basarlarsa en yakın spawn noktasından oyuna devam ederler.

![Target Area](https://github.com/berkanserbes/OyunProgramlama_FinalProjesi/blob/main/ScreenShots/fireLaser.png?raw=true)

### Kutu bölümü

Bu kısımda oyuncular karşıdan gelen kutulardan kaçıp güvenli bölgelere ilerleyerek bu kısmı aşmak zorundadır. Eğer oyuncular kutu nesnesiyle çarpışırlarsa kutu tarafından platformun dışına sürüklenir.

![Box Collision](https://github.com/berkanserbes/OyunProgramlama_FinalProjesi/blob/main/ScreenShots/BoxCollision.png?raw=true)

### Spawn Noktaları

Oyun parkuru bölümlere ayrılmıştır ve bu bölümlerin her bir noktası bir spawn noktasıdır. Oyuncu parkurun dışına düştüğünde veya lazerin üzerine bastığında en yakın spawn noktasından oyuna devam eder.


### 2.Sahne

Oyunculardan herhangi biri birinci sahnenin bitiş noktasına ulaştığında ikinci sahneye geçiş yapılır. İkinci sahne birinci sahnenin aynısıdır.
İkinci oyun sahnesinde parkurun bitiş çizgisine ilk ulaşan oyuncu oyunu kazanır. Oyunun sonunda oyunu kazanan kişiyi gösteren ekran ortaya çıkar ve kullanıcı, ana menü ekranına yönlendirilir.
![Second Scene](https://github.com/berkanserbes/OyunProgramlama_FinalProjesi/blob/main/ScreenShots/sahne2.png?raw=true)
![Winner Screen](https://github.com/berkanserbes/OyunProgramlama_FinalProjesi/blob/main/ScreenShots/winScreen.png?raw=true)


Herhangi bir oyuncu ESC tuşuna bastığında oyun duraklatılır ve durdurma menüsü açılır. Bu durdurma menüsünde 'Devam Et', 'Yeniden Başlat' ve 'Ana Menü' adlı üç adet buton bulunmaktadır. Oyuncu 'Devam Et' butonuna basarak oyuna kaldığı yerden devam edebilir. 'Yeniden Başlat' butonuna basarak oyuna yeniden başlayabilir. 'Ana Menü' butonuna basarak Ana Menü ekranına geçiş yapabilir ya da yeniden ESC tuşuna basarak bu durdurma menüsünü kapatabilir.

![PauseMenu](https://github.com/berkanserbes/OyunProgramlama_FinalProjesi/blob/main/ScreenShots/pauseMenu.png?raw=true)

<hr>

## Oyunu Geliştirenler ve Görevleri

<h3>Samet Özkan</h3>

* Animasyon
* Ses ve Müzik
* Oynanabilir Sahneler

<h3>Berkan Serbes</h3>

* Ana Menü
* Kayıt Alma

## Kullanılan Dosyalar

* <p> Human animasyon: <a href="https://assetstore.unity.com/packages/3d/animations/basic-motions-free-154271">https://assetstore.unity.com/packages/3d/animations/basic-motions-free-154271</a> </p>
* <p> Material: <a href="https://assetstore.unity.com/packages/2d/textures-materials/20-ground-material-sets-sci-fi-12401">https://assetstore.unity.com/packages/2d/textures-materials/20-ground-material-sets-sci-fi-12401</a></p> 
* <p> Background Music: <a href="https://opengameart.org/content/railjet-long-seamless-loop">https://opengameart.org/content/railjet-long-seamless-loop</a></p>
* <p> Spawn Noktası Sound Effect: <a href="https://opengameart.org/content/cute-mission-complete">https://opengameart.org/content/cute-mission-complete</a></p>
* <p> Skill Sesi: <a href="https://opengameart.org/content/spell-4-fire">https://opengameart.org/content/spell-4-fire</a></p>
* <p> Ateş Etme Sesi: <a href="https://pixabay.com/sound-effects/shotgun-firing-4-6746/">https://pixabay.com/sound-effects/shotgun-firing-4-6746/</a></p>
* <p> Zıplama Sesi: <a href="https://pixabay.com/sound-effects/cartoon-jump-6462/">https://pixabay.com/sound-effects/cartoon-jump-6462/</a></p>