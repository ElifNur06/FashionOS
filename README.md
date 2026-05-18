# FashionOS: Dijital Moda Tasarım ve Üretim Ekosistemi 👗✨

FashionOS, bağımsız moda tasarımcıları, butikler ve hazır giyim üreticileri için geliştirilmiş; 3D modellemeden vektörel kalıp çıkarma süreçlerine, yapay zeka destekli kumaş üretiminden mini ERP (iş yönetimi) süreçlerine kadar tüm operasyonları tek bir çatı altında toplayan uçtan uca bir mobil ekosistemdir.

---

## 🚀 Öne Çıkan Özellikler & Modüller

### 1. 3D Atölye Modülü (Atelier Lab Elite)
* **Ready Player Me Entegrasyonu:** Tasarımcıların Ready Player Me üzerinden ürettikleri özel 3D insan modellerini (.glb) URL bağlantısı aracılığıyla doğrudan uygulamaya aktarabilmesini sağlar.
* **Dinamik Animasyon & Morphing:** Aktarılan mankenler üzerinde "Yürü", "Koş", "Dur" ve "T-Poz" gibi animasyonlar pürüzsüzce çalıştırılabilir. Slider'lar yardımıyla mankenin boy ve genişlik gibi vücut oranları gerçek zamanlı olarak değiştirilebilir (Morphing).
* **Manken Canlı Tutma Mimarisi:** Alt sekmeler (Teknik Oda, Pro Tools vb.) arasında geçiş yapıldığında 3D render motorunun sıfırlanmasını ve bellek boşaltılması kaynaklı çökmeleri engelleyen `AutomaticKeepAliveClientMixin` altyapısı kullanılmıştır (`wantKeepAlive = true`). Sayfa değiştirilse dahi manken arka planda asenkron olarak çalışmaya devam eder.
* **Tuval Özelleştirmeleri:** Detay çizimler için çizim tuvali $0^\circ$ ile $360^\circ$ arasında serbestçe döndürülebilir, yakınlaştırılabilir (zoom) veya kaydırılabilir. Etkileşimli jestler, 3D nesneden bağımsız çalışan `TransformationController` ile iki parmak üzerinden yönetilir.
* **Smart Palette (Dinamik Renk Harmonisi):** Çizim fırçalarının altında çalışan renk harmonisi motoru (`HSVColor Harmony Algorithm`), seçilen temel renge göre otomatik olarak tamamlayıcı, analog ve triadik renk kombinasyonları türeterek matematiksel olarak kusursuz couture kartelaları oluşturur.
* **Couture Engine (Gelişmiş Çizim Motoru):** Manken üzerine doğrudan sanatsal efektler çizilmesini sağlar. *Fırça Tipleri:* Normal, Kesik (Dikiş), İnci, Pul/Payet, Altın, Gümüş, Gökkuşağı, Gölgelendirme (`Multiply`) ve Aydınlatma (`Overlay`). Titreme önleyici `Smooth Stabilizer`, radyal simetri ve teknik ölçüm cetveli ile desteklenmiştir.

### 2. Teknik Çizim Stüdyosu (Fashion Tech Studio)
* **Vektörel Bezier Aracı:** Noktalar atarak ve kavis kollarını çekerek fabrikasyon standartlarında kusursuz vektörel kalıplar çizilmesini sağlar. Akıllı Grid (Izgara) yapıştırma motoru milimetrik hizalamayı garantiler.
* **Dinamik Bağlam Menüsü (Context Menu):** Tuval üzerindeki herhangi bir vektör nesnesine uzun basıldığında dinamik bir menü tetiklenir. Seçili katmanı en üst katmana taşıma (`layers.add(item)`) veya kalıcı silme işlemleri bellek seviyesinde asenkron yürütülür.
* **Kilitli Katman Koruması (Security Barrier):** Sağ panelden kilitlenmiş olan (`isLocked = true`) bir katman kazara seçilse dahi, üzerinde çizim kalemi darbesi vurulmasını veya doku kaplanmasını engeller; kullanıcıyı `_showLockedWarning()` interaktif arayüzü ile uyarır.
* **Dikiş Tipleri & Damgalar:** Çizgilere Düz, Kesik Çizgi, Zigzag, Overlok ve Çift İğne efektleri uygulanabilir. Hazır damga (Stamp) menüsünden tasarımlara anında hazır Cep veya Düğme vektörleri basılabilir.
* **Otomatik Tech Pack Çıktısı:** Tasarlanan ürünün; kumaş cinsi, teknik ölçüleri, toleransları, dikiş tipleri ve vektörel kalıplarıyla birlikte anında endüstri standardında bir üretim föyü (PDF) halinde kaydedilmesini, paylaşılmasını ve kablosuz yazdırılmasını sağlar.

### 3. Boyama ve Rendering Stüdyosu
* **Gerçek Zamanlı Doku Menüsü:** Uygulamayı ağırlaştırmayan, yüksek çözünürlüklü ve doğrulanmış bulut tabanlı bir kumaş veritabanı barındırır. Saten, Denim, Deri, Pamuk, Kadife, Keten, Örgü, Yün, Şifon ve Pelüş gibi kumaş dokuları şablonlar üzerinde anında simüle edilebilir.

### 4. Akıllı Tarayıcı ve Laboratuvar (Smart Scanner)
* **Gelişmiş Kamera Katmanları:** Fiziksel kağıttaki çizimleri hatasız aktarmak için dikey çekimlerde kağıdın düz durmasını denetleyen jiroskop tabanlı bir Su Terazisi (`Jiroscop Leveler Painter`) ve ekranda sürekli hareket ederek belge taraması gerçekleştiren dinamik bir tarama çizgisi (`Smart Line Scan Controller`) içerir.
* **Çoklu Tarama Modları & Hayalet Manken:** Kameranın odaklandığı noktanın uluslararası renk kodunu yakalayan canlı HEX Picker (Renk Modu), dikişsiz döşeme (Tile) ve arka plan temizleyen Yapay Zeka destekli "AI Makas" modları sunar. Kamera arkasına transparan bir kılavuz yerleştiren "Hayalet Manken" (`Ghost Mode`) ile kıyafetler doğru açıyla dijitalleştirilir.

### 5. İş Yönetimi ve Pro Tools (Business Hub)
* **Dinamik Maliyet Veritabanı:** Maliyet Sihirbazı, arka planda çalışan dinamik bir kumaş fiyatlandırma matrisi (`fabricPrices`) ile entegre çalışır. Saten, Denim, Pamuk, İpek ve Polyester gibi kumaşların güncel birim fiyatlarını (örn: İpek için 450 TL/m) baz alarak metraj tüketim hesaplamalarını dinamik çarpanlarla işler.
* **AI Beden Serileştirme (Grading Engine):** Tek tuşla M baz bedenden S, L, XL kalıplarını otomatik olarak hesaplar ve üretim tablosuna işler.
* **AI Pattern Maker:** Prompt (yazılı komut) kutusuna girilen ifadelere göre benzersiz, telifsiz ve sıfır maliyetli kumaş desenleri üretir.
* **Portfolio Showroom:** "Portfolyo Yayınla" özelliği sayesinde tasarımları doğrudan kişisel web sitelerine entegre etmek amacıyla anında kopyalanabilir hazır HTML portfolyo kodları üretir.
* **Mini ERP Merkezi:** Aktif sipariş durumlarını (Hazırlanıyor, Kargoda, Bekliyor), kritik malzeme stok seviyelerini (Fermuar, Astar vb.), kayıtlı toptancı rehberini (CRM) ve üretim takvimini (Kumaş teslimatı, Koleksiyon çekimi, Moda haftası) tek ekrandan takip etmeyi sağlar.

---

## 🛠️ Teknik Mimari & Algoritmalar

* **UI/UX Design Framework:** Performans ve göz yormayan bir estetik için tamamen **Aydınlık Moda Teması (Light Theme)** ilkelerine göre geliştirilmiştir.
* **Kullanıcı Deneyimi:** Uygulamaya dahil edilen interaktif *Onboarding* rehberi, tüm donanımsal ve yazılımsal yetenekleri yeni kullanıcılara simüle ederek öğretir.
* **Veri ve Bellek Yönetimi:**
    * `AutomaticKeepAliveClientMixin` ile sekme geçişlerinde 3D Viewport durumunun korunması.
    * `TransformationController` ile UI matris manipülasyonu (Döndürme, Zoom, Kaydırma).
    * Dinamik katman yönetimi için asenkron asılı bellek işlemleri (`layers.add`).
    * Gerçek zamanlı bütçe analizi için `fabricPrices Matrix` çarpan motoru.

---

## 📝 Örnek Üretim Föyü (Tech Pack) Çıktı Formatı

Sistem tarafından otomatik oluşturulan resmi `FASHION OS - TECH PACK` döküman yapısı aşağıdaki hiyerarşiyi takip eder:

* **Meta Veriler:** Proje Adı (Örn: Yaz Koleksiyonu Ceket), Kumaş Tipi (Örn: Saten), Tasarımcı Bilgisi ve Oluşturulma Tarihi.
* **Görsel Alanı:** Teknik Çizim Vektör Matrisi.
* **Ölçü Tolerans Tablosu:**

| Ölçü Noktası | Tolerans | Small (cm) | Medium (cm) | Large (cm) |
| :--- | :--- | :--- | :--- | :--- |
| Yaka Genişliği | 0.5 | 18 | 19 | 20 |
| Göğüs | 10 | 48 | 50 | 52 |
| Boy | 4-5 | 68 | 70 | 72 |

---
## Görseller
<img width="338" height="599" alt="image" src="https://github.com/user-attachments/assets/b84dc1b2-5ad5-40ed-be3b-394691da012c" />
<img width="339" height="593" alt="image" src="https://github.com/user-attachments/assets/dc6ef5d2-439b-42a2-aae2-498f31fe97bf" />
<img width="340" height="598" alt="image" src="https://github.com/user-attachments/assets/5bb625ea-9934-45e2-a364-089df325701a" />
<img width="334" height="598" alt="image" src="https://github.com/user-attachments/assets/b3e30063-20fc-46bd-80b8-2763b5ceab34" />
<img width="334" height="598" alt="image" src="https://github.com/user-attachments/assets/c8b259b0-41bc-474d-9d44-a6df71d3f35f" />
<img width="335" height="594" alt="image" src="https://github.com/user-attachments/assets/d1e717a2-3e3f-4a54-bd34-e11f7a4624bd" />
<img width="337" height="596" alt="image" src="https://github.com/user-attachments/assets/e9592f6f-e698-4ce5-8cef-94fff5e8aee0" />
<img width="338" height="594" alt="image" src="https://github.com/user-attachments/assets/946558c4-91d3-43ef-990c-4da0bbe8cda9" />
<img width="335" height="596" alt="image" src="https://github.com/user-attachments/assets/3cb982f4-d055-43f4-8407-f35d1544208c" />
<img width="336" height="595" alt="image" src="https://github.com/user-attachments/assets/368a8b76-f85a-4e6d-8739-8cf610eb589b" />
<img width="338" height="599" alt="image" src="https://github.com/user-attachments/assets/24b3fcb2-92ec-4b9b-a7e8-4f5384485efd" />
<img width="336" height="595" alt="image" src="https://github.com/user-attachments/assets/8fa0e963-fce8-40e4-a76e-8fa4149b4763" />
<img width="337" height="598" alt="image" src="https://github.com/user-attachments/assets/5566cb82-a6c9-4db1-90e6-869fc6ff9eca" />
<img width="337" height="601" alt="image" src="https://github.com/user-attachments/assets/4ae137fb-8485-4e56-b10d-8915c8793ba1" />


## 📄 Lisans ve Dokümantasyon Notu

Bu proje **FashionOS Sürüm 1.0.4 (Nihai Kararlı Versiyon)** teknik dokümantasyon spesifikasyonlarına göre tasarlanmış ve üretilmiştir. Tüm hakları saklıdır.  
*Dokümantasyon Tarihi: Mayıs 2026*
