<p>Videoda &Ouml;rnek node kurulumuda yaptık izlemek isterseniz <a href="https://youtu.be/LrJvtA90PUE">TIKLA</a></p>

<p><strong>1 &mdash;Node Kurmak Ne kadar zor ?</strong></p>

Node kurması gerçekten çok kolaydır..Kafanızdaki düşünceleri çok iyi biliyoruz bizde bu yollardan geçtik .. İşin içine girdiğiniz vakit ne kadar kolay olduğunun farkına varacaksınız.. En basitinden şöyle örnek verebiliriz bir markette çalışan olarak girdiniz bazı şeyleri öğrenmeniz ve alışkanlık haline getirmeniz 1–2 hafta sürecektir bunuda o şekilde düşünebilirsiniz..Bir an önce bir ucundan tutun ve node kurulum işlemlerine başlamanızı şiddetle öneriyoruz..

<p><strong>2 &mdash; Bilgisayarımdan node kurabilirmiyim ?</strong></p>

Node kurulumunu kendi bilgisayarınıza kurabilirsiniz Fakat kurmanızı Önermiyoruz …

<p><strong>&middot; </strong> Bilgisayarınız 7–24 açık kalmak zorunda kalacak.
<p><strong>&middot; </strong>kendi internet hızınız çok yavaş olucak . Sunucuların internet hızı normal internet hızlarından kat kat yüksektir.
<p><strong>&middot; </strong>Kendi bilgisayarınıza node kurarsanız diskiniz dolmaya başlayacak ve bir zamandan sonra zorluk yaşamaya başlayacaksınız..
<p><strong>&middot; </strong>internet kopmasında veya elektrik kesintisinde kurulum yaptığınız node çalışır vaziyette olmayacak..
<p><strong>&middot; </strong>NodesWizard ekibi olarak asla kendi bilgisayarımıza node kurmuyoruz ve sizlerede önermiyoruz..
  
<p><strong>3 &mdash; Bilgisayarımızdan Node kurulum yapamayacağız peki nereye kurulum yapacağız ?</strong></p>

<p><strong>&middot; </strong>Node kurulum işlemlerinde VPS yani uzak sunucu bağlantısı yaparak kurulum işlemleri yapacağız..
<p><strong>&middot; </strong>Ücretsiz olarak Temin edebileceğiz en sağlam ve en bilinir yerler Digital Ocean , Google Cloud , Microsoft Azure ve Amazon AWS’dir.
<p><strong>&middot; </strong>Ücretli olarak temin edebileceğiniz ve bizimde şuan 1. olarak olarak tercih ettiğimiz yer Hetzner’dir .. Çok zorda kalırsak ve limit sıkıntısı yaşarsak Contabo kullanıyoruz..
<p><strong>&middot; </strong>Sunucumuzu nereden açarsak açalım Ubuntu 20.04 işletim sistemini seçerek açıyoruz..
<p><strong>&middot; </strong>Buralara nasıl üye olunur ücretli ve ücretsiz nasıl sunucu açılır aşağıdaki linklerden ulaşabilirsiniz..
  
<p>Digital Ocean : <a href="https://medium.com/@nodeswizard/digital-ocean-kay%C4%B1t-olma-ve-%C3%BCcretsiz-sunucu-olu%C5%9Fturma-i%C5%9Flemleri-919adbc71aa8">TIKLA</a></p>
<p>Google Cloud : <a href="https://medium.com/@nodeswizard/google-cloud-kay%C4%B1t-olma-ve-%C3%BCcretsiz-sunucu-a%C3%A7ma-i%C5%9Flemleri-12f067f3caeb">TIKLA</a></p>
<p>Microsoft Azure : <a href="https://medium.com/@nodeswizard/microsoft-azure-%C3%BCcretsiz-sunucu-nas%C4%B1l-a%C3%A7%C4%B1l%C4%B1r-8cfa3a3d06a4">TIKLA</a></p>
<p>Amazon AWS : <a href="https://medium.com/@nodeswizard/%C3%B6nemli%CC%87-not-nodeswizard-ekibi-olarak-amazon-aws-yi-sadece-free-sunucu-se%C3%A7ene%C4%9Fi-ile-a%C3%A7man%C4%B1z%C4%B1-ve-58b7465143d8">TIKLA</a></p>
<p>Contabo : <a href="https://medium.com/@nodeswizard/contabo-sunucu-sat%C4%B1n-alma-ve-detayl%C4%B1-kullan%C4%B1m-d7dcf53b8818">TIKLA</a></p>

<p><strong>4 &mdash; Sunucuyu Temin ettik şimdi nasıl kurulum yapacağız?</strong></p>

Sunucuyu temin ettikden sonra ip adresiniz, kullanıcı adınız ve şifreniz olur. kullanıcı adınız genellikle root olur .. Şifreyi kendiniz belirlersiniz ve IP adresiniz sağlayacı firma tarafından size random verilir.. Şimdi bu sunucumuza bağlanmak için bize bunu sağlayacak aracı programlar lazım olacaktır.

<p><strong>&middot; </strong>Termius : NodesWizard ekibi olarak Termius kullanmaktayız ve size kesinlikle bağlantı için Termius öneriyoruz…Windows ve MAC bilgisayarınıza hatta telefonunuza indirebilir oradan da node kurulumu yapabilirsiniz..
  
Termius video : https://youtu.be/tIG7kCDgyGw

<p><strong>&middot; </strong>Putty : Putty arada kullandığımız bir programdır .. Termius çıtayı çok yükselttiği için ve mükemmel olduğu için putty kullanmıyoruz..Putty’nin yardımcı programı puttygen bazı konularda lazım olduğu için Putty kurulumunu sizlere öneriyoruz..Putty kurduğunuzda puttygen yanında otomatik olarak kurulmaktadır..
  
Putty video : https://youtu.be/dxCFKpecIHU

Sunucuya bağlandığımızda Node kurulumlarını genel olarak otomatik script ile yapıyoruz.. Fakat siz her ihtimale karşı sunucuya ilk giriş yaptığınızda 1 kereliğine aşşağıdaki kod ile sunucunuzu güncelleyiniz..
```
sudo apt update && sudo apt upgrade -y
```
<p><strong>5 &mdash; Node testnet kazan&ccedil;ları ve s&uuml;releri?</strong></p>

Node Testnetleri ne kadar sürer ;

Bu konuda ne söylersek kendimizi kandırmış oluruz .. Ağda bir sorun olur veya testten istenilen verim alınamaz testnet uzar yada 2. ve 3. çıkarılarak bu durum bu şekilde uzayabilir..O yüzden testnetlere büyük beklentiyle girmemek gerekiyor .. Kısa sürede biter diyerek girmemeniz gerekiyor .. Beklentinizi hiç bir zaman çok yüksek tutmayın.. Sonra büyük hayal kırıklığına düşersiniz .. Bu işler hiç belli olmaz ummadık taş baş yarar.. Hiç birşey vermicek dediğimiz bir testnet bir anda çıkar binlerce dolar ödül dağıtabilir..

<p><strong>&middot; </strong> Forta 1.5 ay gibi süre diliminde 5000+ dolar ödül dağıttı ve hala haftalık ödül dağıtmakta…Testnete katılım çok kolaydı.
<p><strong>&middot; </strong> Quicksilver ortalama 15 gün sürecekti fakat ağ çok sorunlu olduğu için 25 gün sürdü.. Ödüller açıklandı ve NodesWizard ekibi olarak 17.000 adet token kazandık .. Katılan herkes yaptığı görevlere göre çeşitli ödüller kazandı..Ödüller ağustos sonunda dağıtılacak.
<p><strong>&middot; </strong> Massa testneti ise 1 yıldır sürüyor.. 1 yıl önce aktif olan test hala devam ediyor..ağustos ayı itibariyle 13. etap devam ediyor ve artık bitmesine çok az kaldı.
<p><strong>&middot; </strong> Celestia testneti devnetten beri hesaplarsak 2023 Q1 e kadar süreceği düşünülüyor.. buda koskoca 1 yıl demek..
<p><strong>&middot; </strong> Sei network ödüllü testnet 9 hafta sürmesi planlanıyor ..
<p><strong>&middot; </strong> Kujira testneti 25 gün civarı sürdü . Aktif setten seçilen kişilere mainnette validatör yaptılar ve o kişilere 200.000 adet kujira stake edildi..
<p><strong>&middot; </strong> Aptos AIT 2'ye 200 kişi seçildi.. Türkiye’den sadece 2 kişi seçilebildi..Seçilenler 500 aptos ödül alacaklar .. Aptosun 350 M dolar yatırım aldığı düşünülerse ödül çok fazla değerli olacak…
<p><strong>&middot; </strong> AVAX testnetine kullanıcılarına 2000 adet token verdi.. o zamanki fiyatı kaçtı bilmiyoruz fakat insanlar çok çok iyi kazandılar.
<p><strong>&middot; </strong> Casper Network sanırım bilmeyen çok az kişi vardır ..Katılan kişilere ortalama 6 ay boyunca aylık 400–500 Euro civarı para verildi..Yani toplamda 3000 euro diyebiliriz..
<p><strong>&middot; </strong> Hopr testnet katılımcılarına 0.05'den 16 k adet token alım hakkı verdi…Tokenin şuanki bozuk piyasada bile fiyatı bile 0.11…Token 2.23 dolar ile ATH yaptı … Bu testnete katılanlar 800 dolara aldıkları 16 k tokeni minimum 15–20 katına sattı ..Bu testnete girenler minimum 10000+ dolar kazandılar..
<p><strong>&middot; </strong> Polymath katılımcıların 2500 adet token verdi .. Tokenin ATH değeri 1.58 dolar ..bu tokeni ortolama 0.8 dolardan satıldığını düşünürsek 2000 dolar katılımcılar ödül kazandılar..
<p><strong>&middot; </strong> Vega protocol testnetine katılımcılarına 20+ Vega token verildi.. ATH değeri 20 dolar civarlarında olan token kilitli olarak verildi..Ortalama 10 dolardan satılarak 200 dolar civarı ödül alındı.
<p><strong>&middot; </strong> Kira testnetine katılanlarına 500 dolar civarı ödül dağıtttı.
<p><strong>&middot; </strong> Umee Ico’dan alım hakkı verdi .. Umee bu konuda baya popüler platform testnetinde bile katılımcılarına 80 dolarlık token verdi..Umee testnetine katılanlar çok iyi kazançlar sağladı.
<p><strong>&middot; </strong> NYM 1250 token ayrıca Ico’dan alım hakkı vermiştir.. Şuan fiyatı 0.39 olsada katılımcıların bu tokeni 1+ dolardan sattı…Ayrıca Ico’dan alım hakkı verildiği için testnete katılanlar minimum 2000+ dolar kazanç sağladı..
<p><strong>&middot; </strong> MINA‘yı bilmeyen yoktur sanırım .. MINA gibi popüler olan bir testnete katılırsanız hayatınız tamamen değişebilir…Minaya katılanlarda 60 bin civarı token aldılar… Tokenlerin çoğu kitli olmasına rağmen bu katılımcıların çok daha işine yaradı..Bekledikçe fiyat artmaya devam etti..bu testnete katılanlar 75 bin+ dolar ödül kazandılar..
<p><strong>&middot; </strong> Moonriver testnet katılımcılarına 20–100 arası token verdi ..Kişilerin aktifliğine göre yaptığı görevlere göre ödül dağılımı oldu.. Moonriver 400 + dolar ATH yaptığını düşünürsek epey bir kazanç edildiğini görebiliyoruz . Ortalama 50 adetten tanesi 200 dolar bile hesaplasanız 10000 dolar para yapıyor.. Testnete katılımcılarından bazıları 30-40 bin dolarlara kadar kazandıklarını söylemeden geçmeyelim.
<p><strong>&middot; </strong> Azero : Bu testnete katılanlar ön satış fiyatından 300 dolarlık token aldılar.. Yaklaşık 8–10 bin dolar civarı kazanç sağlandı.
<p><strong>&middot; </strong> Sadece iyileri söylemek olmak birazda kötülerden örnek verelim .. Streamr katılımcılarına 10 dolar verdi .. Spacemesh katılımcılarına şapka çorap yolladı..Ayrıca birçok testnet katılımından ödül alınmadan eli boş dönülmüştür..
Telegram kanallarımız ;

Sohbet : https://t.me/nodeswizard

Duyuru : https://t.me/nodeswizardduyuru

Website : https://www.nodeswizard.com

Twitter : https://twitter.com/NodesWizard

Github : https://github.com/NodesWizard
  
Linktr : https://linktr.ee/nodeswizard
