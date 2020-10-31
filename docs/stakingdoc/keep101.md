# Ağı Tut 101

Keep Network, özel anahtar gibi dağıtılmış küçük miktarlarda veriyi "depolayan" bir gizlilik çözümüdür. Random Beacon ve t-ECDSA Keeps, web'in temel teknolojisidir.

## Keep nedir?
Keep, bir veya daha fazla sağlayıcı veya katılımcı arasında paylaşılan 1MB'ye kadar şifreli depolama alanıdır. Keep Provider, Keep Ağındaki bir ekonomik varlıktır; bir hissesi vardır ve bir imzalama grubuna imzalayan olarak katılabilir

KEEP, Keep Network'ün ana belirtecidir. Web'deki tüm uygulamalar bunun üzerine inşa edilir veya kurulacaktır.

Keep Network, imzalama grubu oluşturma süreci için güvenilir bir rastgelelik kaynağına dayanır. İmza sahiplerinin seçimi rastgele. Bu güvenilir rastgelelik kaynağı, Rastgele İşaret olarak da adlandırılan BLS Eşik Rölesidir.

## Random Beacon nedir?
Keep çözümü, küçük miktarlarda veriyi (örneğin, bir özel anahtar) gizli tutma yeteneğine dayanmaktadır. Gerçek rastgelelik bu yüzden çok önemlidir. Tüm taraflar, kullanıcının ne üzerinde çalıştığını bulmak için işbirliği yapmak zorunda kalacak ve katılımcıların seçimi gerçekten rastgele olduğunda gizli anlaşma neredeyse imkansız hale geliyor.
Random Beacon, hem ağdaki hem de Ethereum zincirindeki saldırganlara dirençli, doğrulanabilir rastgelelik yaratmanın bir yoludur. İmzalayan grupları için üye tanımlamak için kullanılır.

> Teknik dokümantasyondan Random Beacon hakkında daha fazla bilgi edinin.

Rastgele İşaret kullanılarak seçilene kadar imzalayanların kendileri de dahil olmak üzere imzalayanların kim olacağını kimse bilemez. Bu, imzalayanların para çalmak veya ağa saldırmak için işbirliği yapmamasını sağlar, bu nedenle işaretçi tarafından sağlanan gerçek rastgelelik çok önemlidir.

Keep Network üzerine kurulu ilk uygulama olan tBTC'nin güvenilirliğini sağlamanın önemli bir yolu, karşı taraf riskini ortadan kaldırmaktır. TBTC'nin işlemleri güvenilir bir aracı olmadan işlemesine izin veren bir imza grubu sistemi kullanır. Bu nedenle, imzalayanın seçimi tBTC'nin düzgün çalışması ve t-ECDSA havuzlarının oluşturulması için çok önemlidir.

## t-ECDSA Keeps nedir?
t-ECDSA keep, Keep Network üzerine kurulu ilk uygulama olan tBTC'nin arkasındaki teknolojidir.

> Teknik dokümantasyonda tBTC hakkında daha fazla bilgi edinin.

SMPC ile uygulanan t-ECDSA tutma, bir dizi coğrafi olarak dağınık varlıklarla (imzalayanlar) işlem imzalayarak sözleşmelerin zincirler arasında veri alışverişi yapmasına izin verir. T-ECDSA, birden çok imzalayan tarafından bağımsız olarak depolanan birden çok ayrı özel anahtarla işlemleri güvence altına alır.

Merkezi olmayan imzalama, herkese açık özel anahtarları ifşa etmeden hesaplamak için sMPC kullanılarak gerçekleştirilir. İmzalama sorumluluğu bölünmüştür ve belirli sayıda katılımcının anahtarlarını kullanarak bir imza oluşturması gerekir.

### Diğer zincirler arası jeton planları hakkında bilgi almak ister misiniz?
Diğer ağlara bir köprü kurmaya yönelik henüz kesin bir plan yok. Ancak Cross-Chain Group, Cosmos, Zcash ve Polkadot gibi kişilerle bu konuda görüşmelerde bulunuyor.

## KEEP: Ağ jetonunu saklayın
Keep Network'e üye olmak için KEEP tokenlerinin bakiyesi gereklidir. Üyeler, platform üzerinde çalışma yaparak ödül almaya hak kazanır. Yapıcı davranışı teşvik eden, verimliliği ve güveni teşvik eden ve Keep Network'ün kabulünü ve büyümesini teşvik eden önemli bir teşviktir.

KEEP, mülkiyeti ağdaki temel işlevleri gerçekleştirme hakkı veren çalışan bir belirteçtir. Token sahipleri, katılmaya uygun olmak için teminat olarak minimum miktarda KEEP delege etmelidir.

Bir delegenin seçildiği çalışma miktarı, delege edilen KEEP'lerin sayısı ile orantılı olacaktır. Örneğin, 1000 KEEP'i delege eden bir kişi, zamanla, 100 KEEP'i delege eden bir kişiden on kat daha sık seçilmeyi bekleyebilir ve başarıyla yaptıkları işle orantılı olarak ödüllendirilecektir.

## Ödüller ve kısaltmalar
Sahipler için KEEP tokenlerinin avantajı, devredilen hisse miktarına bağlıdır. Fikir, daha fazla hisseye sahip olanların daha fazla ödül alacağıdır.

Keep ve tBTC sistemlerindeki kısaltmanın amacı cezalandırmak değil, ağ güvenliğini kötü niyetli davranışlardan korumaktır.
Ödüller ve indirim özellikleri hakkında daha fazla bilgi edinmek için bir sonraki bölüme geçin.

`Keep Team'in resmi belgelerinden alınmıştır.` [Kaynak] (https://keep-network.gitbook.io/staking-documentation/)
`Çevirmen: milosl22`
