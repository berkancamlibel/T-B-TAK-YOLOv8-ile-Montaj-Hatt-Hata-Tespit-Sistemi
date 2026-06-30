TÜBİTAK 2209-A: YOLOv8 ile Montaj Hattı Hata Tespit Sistemi

Bu proje, enerji mekanizmaları montaj hatlarında manuel görsel denetimden kaynaklanan hataları ve zaman kayıplarını önlemek amacıyla geliştirilmiş derin öğrenme tabanlı bir bilgisayarlı görü (computer vision) sistemidir.

TÜBİTAK 2209-A Üniversite Öğrencileri Araştırma Projeleri Destekleme Programı kapsamında başarıyla yürütülmüştür.

a-) Projenin Çarpıcı Sonuçları

1-) Zaman Optimizasyonu: Geleneksel yöntemde operatör tarafından 240 saniye (4 dakika) süren manuel gözle kontrol işlemi, bu sistem sayesinde 20 saniyeye -düşürülmüştür. (%91'lik operasyonel zaman tasarrufu)

2-) Yüksek Başarı Oranı: Tamamen gerçek saha koşullarından toplanan karmaşık verilerle eğitilen model, %86.7 başarı (F1 Skoru) elde etmiştir (0.429 güven eşiğinde).

3-) Endüstriyel Uygulanabilirlik: Sistem, pahalı ve endüstriyel kameralar yerine standart mobil cihazlarla toplanan görüntüler üzerinden optimize edilerek düşük maliyetli bir çözüm sunmuştur


b-) Kullanılan Teknolojiler

1-) Yapay Zeka & Derin Öğrenme: YOLOv8 (Ultralytics)
2-) Görüntü İşleme: OpenCV, Python
3-) Veri Etiketleme: LabelImg

c-) Sistem Mimarisi ve Akış

Projede sentetik (CAD vb.) veriler kullanılmamış; model tamamen fabrikanın üretim bandından elde edilen yansımalı, gerçekçi ve karmaşık görüntülerle eğitilmiştir. Toplamda 1373 eğitim ve 176 test verisi kullanılmıştır.
<img width="1665" height="584" alt="image" src="https://github.com/user-attachments/assets/5769ee06-80b4-4afd-a9af-e00a9ef8c82f" />

d-) Performans Metrikleri

Modelin performansı çeşitli güven eşiklerinde test edilmiş olup, en ideal doğruluk ve duyarlılık dengesi (F1-Confidence) aşağıdaki gibi ölçülmüştür:
<img width="2250" height="1500" alt="BoxF1_curve" src="https://github.com/user-attachments/assets/77571c45-3069-4668-ae50-f3216d730ec9" />
