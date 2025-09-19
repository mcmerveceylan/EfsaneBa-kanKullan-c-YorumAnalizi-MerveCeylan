Efsane Başkan - Kullanıcı Yorum Analizi
 **Proje Amacı:
 "Efsane Başkan" oyununun Google Play yorumlarını analiz ederek kullanıcı memnuniyeti trendlerini ve sık rastlanan şikayetleri ortaya çıkarmak.
 **Kullanılan Teknolojiler:
 Python, pandas, matplotlib, nltk, wordcloud, google-play-scraper, re, Counter
 ** Analiz Adımları
1. Google Play Store’dan yorumların çekilmesi (`google-play-scraper` kullanılarak)
2. Yorumların temizlenmesi (stopwords, emoji temizleme)
3. **Duygu Analizi** (Pozitif / Nötr / Negatif) → VADER + Türkçe özel kelime listesi
4. **Kelime Frekansı Analizi** → en çok kullanılan kelimeler
5. **Zaman Serisi Analizi** → güncellemelerden önce/sonra duygu değişimi
6. Görselleştirmeler (bar grafikleri, zaman serisi grafikleri, opsiyonel kelime bulutu)
 **Sonuç
 -Zaman serisi analizi, son güncellemelerden sonra pozitif yorumlarda düşüş olduğunu gözlemleniyor.Gelecek güncellemelerde kullanıcı geri bildirimleri ve kelime analizi baz alınarak, oyuncuların daha çok beğendiği özellikler ve oyundaki teknik sıkıntılar geliştirilmeye odaklanılabilir.
 -Pozitif ve nötr yorumlar oluşurken, negatif yorumlar hiç oluşmuyor.Bu da kullandığım VADER (duygu analiz aracı) Türkçe için yeterli olmayışından kaynaklı.Bunun yerine makine öğrenmesi algoritlarından ya da özel kelime listeleri ve LLM/transformer tabanlı modellerle doğruluk artırılabilir.
 
