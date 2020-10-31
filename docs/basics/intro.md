# TBTC'ye Giriş ve Ağı Koru


## DeFi
Merkezi Olmayan Finans (DeFi), Ethereum ağında oluşturulan ve işletilen açık ve birbirine bağlı finansal hizmetler ve ürünler sistemidir. Temmuz 2020'ye kadar, merkezi olmayan akıllı sözleşmeler yoluyla krediler, belirteçler, türevler, borsalar sunan tüm DeFi uygulamalarında yaklaşık 4 milyar dolar yer alıyor. Bu hacim büyümeye devam ediyor.

DeFi protokolleri, birbirleriyle etkileşime girerek giderek daha karmaşık bir sistem oluşturan modüler bir yapıya sahiptir. DeFi ürünleri, Ethereum gibi bir blockchain ağında bulunan kodlar olduğundan, bunları kullanmak isteyen hiç kimseden asla devre dışı bırakılamaz veya gizlenemez. Böylece, İnternet erişimi olan herkes, DeFi'de borç verme, kapsamlı finansal ürünler, tasarruflar, yatırım ve ticaret fırsatlarından yararlanabilir.

## Niyetler tBTC
DeFi ve Ethereum'daki projelerin katlanarak büyümesine rağmen, bitcoin hala dünyadaki toplam kripto para birimi hacminin üçte ikisini oluşturuyor.

Ilyas Khatsis'in [blogunda] (https://medium.com/@iliashatzis/could-bitcoin-on-defi-displace-banks-yes-4c0ad99f0da4) tBTC'yi tanıttığı gibi:
> "Bitcoin DeFi, bitcoin meraklılarının hayalidir. Hayal kurabiliriz ve yeni tBTC projesi Bitcoin'i DeFi dünyasına getirecek.
> Bitcoin, DeFi'yi çarpıcı bir şekilde dönüştürme potansiyeline sahip ve Keep ekibi bunu anlıyor. "

Keep ekibi, BTC'ye 1: 1 oranla TBTC Ethereum ERC-20 jetonlarındaki bitcoin'ler için merkezi olmayan, güvenli ve sigortalı bir depolama sistemi olan tBTC'yi başlattı. BTC'lerini Ethereum ve DeFi üzerinde harcamak isteyen Bitcoin sahipleri, emanetçilere (imzalayanlar) güvenmemelidir çünkü imzalayanların gözaltında tuttukları BTC'nin değerini aşan bir teminat vermeleri gerekir.

?> Discord'daki Artem # 4718'den bu konuda mükemmel [video] (https://www.youtube.com/watch?v=cfmQiArg3B8).

İmzalayanlar, daha geniş imzalayanlar ağından rastgele seçilir ve üçlü gruplar halinde çalışır. Teminat, dolandırıcılık veya yetersiz teminat durumunda teminatlarını kaybetme riski ile sistemdeki imza sahiplerinin davranışlarının adil kalmasını sağlar. İmzalayanlar fonları yetkisiz olarak hareket ettirir ve BTC'den daha fazla TBTC'yi gözaltında bırakırsa, sistem, TBTC eşdeğerini piyasadan satın almak ve yok etmek için teminatlarına el koyacak ve TBTC ve BTC varlıklarını dengeye getirecektir.

<p align = "center">
  <img width = "619" alt = "İşaret" src = "https://user-images.githubusercontent.com/68087535/88100735-57075f80-cb73-11ea-996f-ec2d9590b073.png">
</p>


## Ağı Koru

tBTC, Ben Longstaff'ın harika bir [açıklama] (https://medium.com/@ben_longstaff/secure-multi-party-computation) verdiği [Ağı Koru] (https://keep.network) adresindeki bir uygulamadır. -smpc-görsel olarak açıklandı-ecde155fc7c0):

> "Keep Network, verileri ağ dışında güvenli bir şekilde depolamak için bir gizlilik çözümü haline gelirken, akıllı sözleşmelerin işlevselliğini ve blok zinciri teknolojisinin kitlesel olarak benimsenmesini önemli ölçüde genişletmeyi amaçlıyor."

Keep Network, özel anahtar gibi küçük miktarlarda dağıtılmış veriyi depolayan ve zincirler arası iletişimi sürdüren bir gizlilik çözümüdür. Keeps, diğer akıllı sözleşmelerin kişisel verilerle güvenli bir şekilde etkileşime girmesine izin veren akıllı sözleşmelerdir. Önde gelen birçok blok zinciri tarafından desteklenen ECDSA algoritması üzerine inşa edilmişlerdir ve merkezi olmayan grupların çok partili eşik imzaları ile imzalanmasını kolaylaştırırlar.

Ağı [Messari] adresinde tutun (https://messari.io/article/announcement-messari-adds-11-new-disclosures-registry-participants-surpassing-50-members) açık kayıtlı bir üyedir. Bu deftere katılarak, bu projeler kendilerini sürekli açıklama yoluyla kripto varlıkların şeffaflık seviyesini artırmaya adadılar.

[Keeps Grants Explorer] (https://explorer.keep-grants.info/), MutedTommy # 3155 (Discord'da), KEEP'in tahsis edilen bağışlarını belirteçler halinde takip eder.

### t-ECDSA düğümü

T-ECDSA keep, birden çok imzalayan tarafından tutulan birden çok özel anahtarla işlem güvenliği sağlar. Merkezi olmayan imza, paylaşılan anahtarları ifşa etmeden hesaplamak için sMPC (Güvenli Çok Taraflı Hesaplama) kullanılarak gerçekleştirilir. İmzalarla ilgili sorumluluk bölünmüş durumda ve imza oluşturmak için belirli sayıda katılımcı gerekiyor.

Genel olarak, şu şekilde çalışır: Ethereum akıllı sözleşmesi, Keep Network'ten yeni bir t-ECDSA Keep açmasını ister. Bu mağaza, daha büyük bir imzalayanlar ağı olan sMPC kümesinden rastgele seçilen bir grup imzalayan tarafından tutulur. Bu imzalayanlar, bir anahtar oluşturmak ve bir imza sağlamak için t-ECDSA'yı kullanır. İmzalayanlar, blockchain işlemleri dahil her şeyi imzalayabilir. Bir Ethereum akıllı sözleşmesi, herhangi bir ECDSA tabanlı blok zincirinde bir işlem imzalamayı isteyebilir, Bitcoin bunlardan sadece biridir.

Bu mekanizma güvenilirdir çünkü imzalayanlar bağımsızdır; bunlar bir sMPC kümesiyle bir düğüm başlatan kişi ve kuruluşlardır.

<p align = "center">
  <img width = "319" alt = "İşaret" src = "https://user-images.githubusercontent.com/68167410/88845610-05ca2200-d1aa-11ea-9d8b-400516fed25c.png">
</p>

### Rastgele İşaret düğümü

Rastgele İşaret, ağın başka bir parçasıdır: İmzalayanları bir şekilde rastgele seçmek için merkezi olmayan bir araçtır. Bu işaret, BLSThreshold Relay'dir ve kontrol edilemez veya manipüle edilemez. Grup seçimi için güvenilir bir rastgelelik kaynağıdır. Rastgele bir işaretçi tarafından seçilene kadar, imzalayanların kendileri de dahil olmak üzere imzalayanların kim olacağını kimse bilemez. Bu, imzalayanların fonları çalmak veya ağa saldırmak için işbirliği yapamamasını sağlar, bu nedenle işaretin sağladığı gerçek rastgelelik çok önemlidir.

** Random Beacon ve t-ECDSA Keep ağında çekirdek tutar. **



***

** Kaynaklar ve faydalı bilgiler: **
- [DeFi üzerindeki Bitcoin bankaların yerini alabilir mi? Evet] (https://medium.com/@iliashatzis/could-bitcoin-on-defi-displace-banks-yes-4c0ad99f0da4), Ilias Hatzis tarafından
- Keep Network Blog'dan [Bitcoin ve Ethereum Köprüleme] (https://blog.keep.network/bridging-bitcoin-and-ethereum-b2f9923630a7)
- [Güvenli Çok Taraflı Hesaplama] (https://medium.com/@ben_longstaff/secure-multi-party-computation-smpc-explained-visually-ecde155fc7c0), Ben Longstaff
- [tECDSA ile Blockchain'ler arasında Köprüler Kurmak] (https://blog.keep.network/building-bridges-between-blockchains-with-t-ecdsa-keeps-e58d6debb8fd) Keep Network Blog'dan Piotr Dyraga
- Keep Network Documentation'dan [Staking Documentation] (https://keep-network.gitbook.io/staking-documentation/)
- tBTC Web Sitesinden [tBTC Teknik Genel Bakış] (https://tbtc.network/developers/tbtc-technical-system-overview/)
- [What's in a beacon] (https://blog.keep.network/whats-in-a-beacon-12c34b0bc078), Keep Network Blog'dan Antonio Salazar Cardozo tarafından
- [Güvenilir Randomness Neden Bu Kadar Önemli?] (Https://blog.keep.network/why-is-trusted-randomness-so-important-c22de1c1c5ee), Keep Network Blog'dan Antonio Salazar Cardozo
- [Threshold ECDSA - Daha güvenli, daha özel çoklu imzalar] (https://blog.keep.network/threshold-ecdsa-safer-more-private-multi-signatures-51153f3e9ed2), Antonio Salazar Cardozo, Keep Network Blog sayfasından Geliştirici Piotr Dyraga'nın 2018 San Francisco Blockchain Haftası'ndan eşik-ECDSA sunumuna devam edin.
- [Defi açıkladı] (https://decrypt.co/resources/defi-decentralized-finance-explained-guide-learn), Decrypt.co tarafından
- [Defi nedir] (https://defipulse.com/blog/what-is-defi/), Defipulse tarafından
- Discord Design Channel'da Lelka Bo'dan [Tanıtım videosunu koruyun] (https://www.youtube.com/watch?v=h2IErqf-VrQ)
- [TBTC: Bitcoin için Yeni Bir Yan Zincir Tasarımı] (https://insights.deribit.com/market-research/a-new-sidechain-design-for-bitcoin/), Deribit Insights'ta Su Zhu tarafından
- Görüntüler SpaceWalker (Discord Tasarım Kanalı), [Ilias Hatzis] (https://medium.com/@iliashatzis) (hikayesinden), Keep Team (Discord Tasarım Kanalı) 'dan alınmıştır.

---
Topluluk tarafından düzenlenen ve eklenen resmi Keep Team belgelerinden kaynak. '[Kaynak] (https://keep-network.gitbook.io/staking-documentation/)'

Yazarlar: Ramaruro, EstebanK`
`Çeviri: nadyakriy`
