---
title: AccessCacheOptions numaralandırma
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1740
url: /tr/python-net/aspose.cells/accesscacheoptions/
is_root: false
---
##  AccessCacheOptions numaralandırma
Veri erişimi için önbellek seçenekleri. | ile birleştirilebilir birlikte birden fazla seçenek için operatör.



AccessCacheOptions türü aşağıdaki üyeleri gösterir:

###  alanlar
| Alan| Tanım|
| :- | :- |
| NONE | Herhangi bir veri erişimi için önbellek yok.|
| ALL | Çalışma kitabındaki her türlü veri erişimi için mümkün olan tüm iyileştirmeleri uygulayın.<br/> Optimize edilmiş erişim sırasında tüm ayarlar ve veriler değiştirilmemelidir.|
| POSITION_AND_SIZE | Nesnenin (Şekil gibi) konumunu ve boyutunu almak için olası optimizasyonu uygulayın.<br/> Optimize edilmiş erişim sırasında satır yüksekliği ve sütun genişliği ayarları değiştirilmemelidir.|
| CELLS_DATA | Hücrelerin değerlerini almak için olası optimizasyonu uygulayın.<br/>Cells verileri (Cell, Satır verileri ve ayarları) sırasında değiştirilmemelidir.<br/>optimize edilmiş erişim, yeni Cell/Row nesneleri de oluşturulmamalıdır (örneğin<br/> [[indexer]](/cells/python-net/aspose.cells/cells/__getitem__/) tarafından).|
| CELL_DISPLAY | Ekranla ilgili sonuçları almak için olası optimizasyonu uygulayın<br/>hücreler([Cell.display_string_value](/cells/tr/python-net/aspose.cells/cell#display_string_value), [Cell.get_style()](/cells/tr/python-net/aspose.cells/cell/get_style), [Cell.get_display_style()](/cells/tr/python-net/aspose.cells/cell/get_display_style), vb.).<br/>Cells veri ve stille ilgili nesneler (Cell/Satır/Sütun stilleri, sütun genişliği vb.) değiştirilmemelidir<br/>optimize edilmiş erişim sırasında.|
| GET_FORMULA | Formül almak için olası optimizasyonu uygulayın.<br/>Formül ifadesini etkileyebilecek tüm veriler ve ayarlar (Çalışma sayfasının adı, Adın metni,<br/> tablonun sütunu vb.) optimize edilmiş erişim sırasında değiştirilmemelidir.|
| SET_FORMULA | Ayar formülleri için olası optimizasyonu uygulayın.<br/>Formül ifadesini etkileyebilecek tüm veriler ve ayarlar (Çalışma sayfasının adı, Adın metni,<br/> tablonun sütunu vb.) optimize edilmiş erişim sırasında değiştirilmemelidir.|
| CALCULATE_FORMULA | Formülleri hesaplamak için olası optimizasyonu uygulayın.<br/>Cells Optimize edilmiş erişim sırasında veriler değiştirilmemeli, yeni nesneler (Cell, Satır vb.)<br/> oluşturulmalıdır([[indexer]](/cells/python-net/aspose.cells/cells/__getitem__/) gibi)).|
| CONDITIONAL_FORMATTING | Koşullu biçimlendirmelerin biçimlendirme sonucunu almak için olası optimizasyonu uygulayın.<br/>Koşullu biçimlendirmelerin (koşullu biçimlendirme ayarları) sonucunu etkileyebilecek tüm veriler ve ayarlar<br/> koşullu biçimlendirmeler, bağımlı hücre değerleri vb.) optimize edilmiş erişim sırasında değiştirilmemelidir.|
| VALIDATION | Doğrulama sonucunu almak için olası optimizasyonu uygulayın.<br/>Doğrulamanın sonucunu etkileyebilecek tüm veriler ve ayarlar (doğrulama ayarları,<br/> bağımlı hücre değerleri vb.) optimize edilmiş erişim sırasında değiştirilmemelidir.|



###  Notlar

Bazı özellikler için, büyük veri setine erişim çok sayıda tekrarlanan ve karmaşık işlem gerektirir.
arama, hesaplama, ...vb ve bu işlemler çok fazla zaman alacaktır.
Genel durumlar için, erişim sırasında tüm bağımlı veriler değişmeden kalır, bu nedenle bazı önbellekler oluşturulabilir ve
erişim performansını iyileştirin.
Bu amaçla, bu API'i sağlarız, böylece kullanıcı ne tür veri erişimine ihtiyaç duyduğunu belirleyebilir.
olası önbelleğe alma mekanizması ile optimize edilecek.


Lütfen unutmayın, farklı seçenekler için farklı veri setlerinin "salt okunur" olması gerekebilir.
Verilere erişim performansı, önbelleğe alma mekanizmasının kullanılması gibi pek çok konuya bağlıdır.
performansının iyileştirileceğini garanti etmez. Bazı durumlar için,
Erişilecek veri setinin küçük olması gibi önbellek kullanmak daha da fazla zamana neden olabilir çünkü
önbelleğe almanın kendisi de belirli bir ekstra zamana ihtiyaç duyar.

###  Ayrıca bakınız
* modül [aspose.cells](..)
