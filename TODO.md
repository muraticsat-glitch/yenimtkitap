# mtkitap — Uygulama TODO

## Kitaplık ve kitap kartları
- [x] Kitaplık ekranında kitap kartları gösteriliyor. Kartta kitap adı, kitap türü, kitabın alınma tarihi, kapak görseli ve toplam sayfa sayısı yer alıyor; kapak görseli cihaz galerisinden seçilebiliyor; kartta okuma ilerlemesi ve yüzde değeri görünüyor.
- [x] Kitap ekleme, düzenleme ve silme akışları çalışıyor.
- [x] Kitap silme işlemi kontrollü onay istiyor ve ilgili geçmiş kaydını oluşturuyor.

## Okuma ilerlemesi
- [x] Her kitap için okunan sayfa sayısı ve okuma tarihiyle yeni okuma kaydı girilebiliyor.
- [x] İlerleme toplam sayfa ve okunan sayfaya göre otomatik hesaplanıyor.
- [x] Okunan sayfalar arttıkça kitap kartındaki ilerleme çubuğu güncelleniyor.
- [x] Kitabın tamamı okunduğunda ilerleme yüzde 100 olarak gösteriliyor.
- [x] Okuma kaydı ekleme, düzenleme ve silme işlemleri kitap geçmişiyle ilişkilendiriliyor.

## Kitap türleri
- [x] Kitap türleri listelenebiliyor.
- [x] Yeni tür eklenebiliyor.
- [x] Mevcut tür düzenlenebiliyor.
- [x] Tür silinebiliyor; kitaplarda kullanılan tür silinirken uygulama güvenli biçimde "Tür yok" gösteriyor.

## Geçmiş sekmesi
- [x] Geçmiş sekmesinde tüm girilen kayıtlar ve yapılan değişiklikler kronolojik olarak görünüyor.
- [x] Geçmiş kaydı düzenlenebiliyor.
- [x] Seçilen bir geçmiş kaydından önceki veri geri yüklenebiliyor.
- [x] Geçmiş kaydı silinebiliyor.
- [x] Geçmiş işlemleri kitap, okuma kaydı, tür ve geri yükleme olarak ayırt ediliyor.

## Kalıcı veri ve yedekleme
- [x] Kitaplar, türler, okuma kayıtları ve geçmiş kayıtları AsyncStorage ile uygulama kapatılıp açılsa da cihazda kalıcı olarak saklanıyor.
- [x] Tüm uygulama verileri JSON dosyası olarak dışa aktarılabiliyor; native’de paylaşım akışı, web Preview’da indirme akışı kullanılıyor.
- [x] Dışa aktarılan JSON dosyası cihazdan veya paylaşım akışından alınabiliyor.
- [x] JSON yedeği içe aktarıldığında kitaplar, türler, okuma kayıtları ve geçmiş verileri geri yükleniyor.
- [x] Geçersiz veya bozuk içe aktarma dosyası mevcut verileri silmeden kullanıcıya hata gösteriyor.

## Marka ve mobil teslim
- [x] Uygulama adı mtkitap olarak kullanılıyor.
- [x] mtkitap için özgün, kare, yuvarlatılmamış köşeli launcher logo hazırlandı ve Expo native marka dosyalarına bağlandı.
- [x] Arayüz portre yönelimli ve tek elle kullanıma uygun tasarlandı.
- [x] Android APK/AAB üretimine uygun Expo projesi ve yapılandırması korunuyor.

## Teknik teslim kanıtı
- [x] TypeScript tanılamaları kayıtlı ve hatasız.
- [x] Metro (8081) ve API (3000) çalışma servisleri doğrulandı.
- [x] Kitaplık, Geçmiş ve Düzenle ekranları 390×844 mobil Preview’da kontrol edildi.
- [x] Kabul edilen kaynaklar Manus canonical main dalına checkpoint olarak gönderildi.

## Yeni okuma ve tamamlanma akışı
- [x] Kitap kartlarında kitaba ait okuma sayfaları ve her okuma kaydının tarihi listeleniyor.
- [x] Toplam sayfa tamamlandığında kitap kartında “Okundu olarak işaretle” butonu görünüyor.
- [x] “Okundu olarak işaretle” akışında tamamlanma tarihi girilebiliyor.
- [x] Tamamlanma tarihi kalıcı kitap verisine yazılıyor ve özel geçmiş kaydı oluşturuyor.
- [x] Tamamlanan kitap, Geçmiş sekmesinde kapak, başlık, okunan sayfa toplamı ve okundu tarihiyle ayrı kitap kartı olarak gösteriliyor.

## Kütüphane ve klavye güncellemesi
- [x] Kitap kartında okunan sayfa ilerledikçe kalan sayfa sayısı da güncelleniyor.
- [x] Okundu olarak işaretlenen kitap kütüphane listesinden çıkarılıp Geçmiş sekmesindeki tamamlanan kitap kartlarına taşınıyor.
- [x] Geçmişteki tamamlanan kitap kartında “Kütüphaneye ekle” seçeneği bulunuyor; seçildiğinde kitap tekrar kütüphane listesine dönüyor.
- [x] Kitap, okuma, okundu tarihi ve geçmiş düzenleme bilgi girişleri ekran klavyesi açıldığında klavye tarafından kapanmayacak şekilde yukarı taşınıyor.
- [x] Geçmiş sekmesinde aşağı ok butonuyla okuma geçmişi/zaman akışına kaydırma yapılabiliyor.

## Son kullanıcı akışı güncellemesi
- [x] Kitap düzenleme ekranı açıldığında kitap adı, tür, alınma tarihi, toplam sayfa ve kapak dahil mevcut bilgiler otomatik dolduruluyor; kullanıcı bunların üzerinden değişiklik yapabiliyor.
- [x] Okuma sayfası giriş ekranında güncel kalan sayfa sayısı gösteriliyor.
- [x] Okundu olarak işaretlenen kitap Geçmişte kapak, ad, tür, alınma tarihi, sayfa bilgisi ve okundu tarihi bulunan bilgi kartı olarak aktarılıyor.
- [x] Sadece tamamlanmamış/okunmakta olan kitapları gösteren “Okuyorum” sekmesi eklendi.
- [x] Kitap okundu olarak işaretlendiğinde Okuyorum sekmesinden kaldırılıyor ve Geçmişte görünür oluyor.

## Raf ve sekme düzeni
- [x] Okuyorum sekmesi yalnızca okumaya başlanmış veya okumaya devam edilen kitapları gösteriyor.
- [x] Okunmayı bekleyen ve okunması tamamlanan kitaplar Kitaplık sekmesinde tutuluyor.
- [x] Kitaplık kartındaki “Okumaya başla” seçeneği kitabı Okuyorum sekmesine taşıyor.
- [x] Okuyorum kartındaki “Okunmak üzere kitaplığa kaldır” seçeneği kitabı Kitaplık sekmesine geri taşıyor.
- [x] Okuyorum sekmesinde kitap okundu olarak işaretlendiğinde kitap tamamlanmış bilgi kartı olarak Kitaplık ve Geçmiş akışlarına yansıyor.
- [x] Sekmeler Okuyorum, Kitaplık, Geçmiş ve Ayarlar sırasına alındı.

## Değerlendirme ve okuma notları
- [x] Kitap ekleme/düzenleme formunda 5 yıldız üzerinden değerlendirme seçilebiliyor ve istenirse temizlenebiliyor.
- [x] Kitapla ilgili açıklama/yorum yazılabilen çok satırlı alan eklendi.
- [x] Yıldız değerlendirmesi ve yorum kitap kartında, tamamlanan kitap kartında ve kalıcı dışa aktarma verisinde korunuyor.
- [x] Kitap okunmaya başlandıktan ve okuma kaydı eklendikten sonra Okuyorum sekmesinden kitaplığa kaldırılabiliyor.
- [x] Okuma kaydı bulunan rafa kaldırılmış kitapta “Okumaya devam et” seçeneği görünüyor; seçildiğinde kitap yeniden Okuyorum sekmesine taşınıyor.

## Okuma kayıtlarını düzeltme
- [x] Okuyorum sekmesindeki her okuma kaydında sayfa sayısını ve okuma tarihini değiştirmek için düzenle aksiyonu bulunuyor.
- [x] Okuma kaydı silinebiliyor; silme sonrasında toplam okunan sayfa, kalan sayfa ve ilerleme yüzdesi yeniden hesaplanıyor.
- [x] Kitaplıktan tekrar okumaya alınan ve eski okuma kayıtları bulunan kitaplarda mevcut kayıtlar Okuyorum sekmesinden değiştirilebiliyor veya silinebiliyor.

## Yazar ve tamamlanan kitap kartları
- [x] Kitap ekleme/düzenleme formunda yazar adı alanı bulunuyor; mevcut yazar bilgisi düzenleme ekranında otomatik geliyor.
- [x] Yazar adı kitaplık kartında ve tamamlanan kitapların Geçmiş kartında gösteriliyor.
- [x] Kitaplık sekmesindeki okunması tamamlanan kitap kartları aktif/bekleyen kitaplardan farklı arka plan, çerçeve ve “OKUNDU · KİTAPLIKTA” bandıyla ayrılıyor.

## Kitap adı görünürlüğü
- [x] Kitaplık, Okuyorum ve Geçmiş kartlarında kitap adlarının iki satırla kesilmesi kaldırıldı; uzun adlar kart içinde satır satır tamamen gösteriliyor.

## Kitaplık sıralaması
- [x] Kitaplık sekmesinde hiç okunmayan kitaplar en üstte gösteriliyor; aynı durumda yeni eklenen kitaplar kendi aralarında en üstte kalıyor.
- [x] Kısmen okunan kitaplar ilerleme yüzdesi arttıkça daha aşağı sıralanıyor; örneğin yüzde 5 okunan kitap hiç okunmayanların altında yer alıyor.
- [x] Okunması tamamlanan kitaplar Kitaplık listesinin en altında gösteriliyor.

## Kitaplıkta değişken kitap tanıtımı
- [x] Kitaplık ekranındaki “Bugünün sayfası” alanı yalnızca Kitaplık rafındaki kitaplardan birini tanıtıyor.
- [x] Kitaplık ekranı her açıldığında veya sekmeye yeniden dönüldüğünde tanıtılan kitap yeniden seçiliyor; birden fazla kitap varsa aynı kitap art arda seçilmemeye çalışılıyor.
- [x] Tanıtım alanında seçilen kitabın adı, varsa yazarı ve okuma ilerlemesi gösteriliyor; kitaplık boşsa genel tanıtım metni korunuyor.

## Bugünün sayfası görsel tanıtımı
- [x] Bugünün sayfası alanında seçilen kitap varsa kitaplıkta kayıtlı kapak görseli gösteriliyor.
- [x] Seçilen kitabın adı ve varsa yazar adı ayrı ve belirgin biçimde gösteriliyor.
- [x] Kitap kapağı yoksa mevcut mtkitap marka görseli yedek olarak kullanılmaya devam ediyor.

## Bugünün sayfası başlık görünürlüğü
- [x] Bugünün sayfasında seçilen kitabın adı için satır sınırı kaldırıldı; uzun kitap adları artık üç satırdan sonra kesilmiyor ve tamamen gösteriliyor.

## Arama, klavye ve Bugünün sayfası gezinmesi
- [x] Kitaplık araması kitap adıyla birlikte yazar adında da arama yapıyor.
- [x] Kitaplık, Okuyorum, Geçmiş ve Ayarlar sekmelerinin ana içerikleri klavye açıldığında KeyboardAvoidingView ile uyumlu biçimde kayıyor.
- [x] Bugünün sayfasındaki kitap adı yüksek kaliteli kelime kırma ve hyphenation kapalı ayarıyla kelime bütünlüğünü koruyor.
- [x] Bugünün sayfasında kitap varken görünen “İncele” aksiyonu seçilen kitabı arama alanına getirip ilgili kitap kartına kaydırıyor.

## Arama temizleme ve sekme geçişi
- [x] Arama alanında metin varken görünen X butonu metni temizliyor.
- [x] X butonuna basıldığında filtre kaldırılıyor ve tüm kitaplar yeniden görüntüleniyor.
- [x] Kitaplık sekmesinden başka sekmeye geçildiğinde arama metni ve tür filtresi sıfırlanıyor; Kitaplık sekmesine dönünce tüm kitaplar gösteriliyor.

## Ulaşılan sayfa ile günlük okuma hesabı
- [x] Okuma girişinde kullanıcıdan o oturumda okuduğu miktar yerine kitapta ulaştığı son sayfa isteniyor.
- [x] Uygulama önceki ulaşılan sayfayı karşılaştırıp o gün okunan sayfa sayısını otomatik hesaplıyor.
- [x] Günlük fark ve ulaşılan son sayfa kalıcı okuma kaydı olarak saklanıyor.
- [x] İlerleme çubuğu ve kalan sayfa hesabı ulaşılan en son sayfaya göre güncelleniyor.
- [x] Kitap kartındaki okuma kayıtlarında günlük okunan sayfa ile ulaşılan sayfa birlikte gösteriliyor.
- [x] Mevcut eski yedeklerdeki kayıtlarda geriye dönük uyumluluk korunuyor; `currentPage` olmayan kayıtlar önceki toplam sayfa mantığıyla okunuyor.
- [x] Okuma kaydı düzenleme ekranında ulaşılan sayfa değiştirildiğinde günlük fark yeniden hesaplanıyor.
