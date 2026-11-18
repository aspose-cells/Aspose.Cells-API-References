---
title: "AccessCacheOptions Enum"
linktitle: "AccessCacheOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "AccessCacheOptions enum. Go dilinde accesscacheoptions'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/accesscacheoptions/
---

## AccessCacheOptions Enum

Veri erişimi için önbellekleme seçenekleri. Birden fazla seçenek "|" operatörü kullanılarak birleştirilebilir.

```go

type AccessCacheOptions int32


```

## Alanlar

| Alan | Açıklama |
| --- | --- |
| [None](./none/) | Herhangi bir veri erişimi için önbellek yok. |
| [All](./all/) | Çalışma kitabındaki tüm veri erişimi türleri için mümkün olan tüm optimizasyonları uygula. Optimizasyonlu erişim sırasında tüm ayarlar ve veriler değişmemelidir. |
| [PositionAndSize](./positionandsize/) | Nesnenin (örneğin Shape) konum ve boyutunu alırken mümkün olan optimizasyonu uygula. Satır yüksekliği ve sütun genişliği ayarları optimizasyonlu erişim sırasında değişmemelidir. |
| [CellsData](./cellsdata/) | Hücre değerlerini alırken mümkün olan optimizasyonu uygula. Hücre verileri (Hücre ve Satır'ın veri ve ayarları) optimizasyonlu erişim sırasında değişmemelidir, ayrıca yeni Hücre/Satır nesneleri (örneğin <see cref="Cells.this[int, int]"/> ile) oluşturulmamalıdır. |
| [CellDisplay](./celldisplay/) | Hücrelerin (<see cref="Cell.DisplayStringValue"/>, <see cref="Cell.GetStyle()"/>, <see cref="Cell.GetDisplayStyle()"/>, vb.) görüntüyle ilgili sonuçlarını alırken mümkün olan optimizasyonu uygula. Hücre verileri ve stil ile ilgili nesneler (Hücre/Satır/Sütun stilleri, sütun genişliği vb.) optimizasyonlu erişim sırasında değişmemelidir. |
| [GetFormula](./getformula/) | Formülleri alırken mümkün olan optimizasyonu uygula. Formül ifadesini etkileyebilecek tüm veri ve ayarlar (Çalışma sayfasının adı, Adın metni, tablonun sütunu vb.) optimizasyonlu erişim sırasında değişmemelidir. |
| [SetFormula](./setformula/) | Formülleri ayarlarken mümkün olan optimizasyonu uygula. Formül ifadesini etkileyebilecek tüm veri ve ayarlar (Çalışma sayfasının adı, Adın metni, tablonun sütunu vb.) optimizasyonlu erişim sırasında değişmemelidir. |
| [CalculateFormula](./calculateformula/) | Formülleri hesaplarken mümkün olan optimizasyonu uygula. Hücre verileri optimizasyonlu erişim sırasında değişmemeli, ayrıca yeni nesneler (Hücre, Satır vb.) (örneğin <see cref="Cells.this[int, int]"/> ile) oluşturulmamalıdır. |
| [ConditionalFormatting](./conditionalformatting/) | Koşullu biçimlendirmelerin biçimlendirme sonucunu alırken mümkün olan optimizasyonu uygula. Koşullu biçimlendirmelerin sonucunu etkileyebilecek tüm veri ve ayarlar (koşullu biçimlendirme ayarları, bağımlı hücre değerleri vb.) optimizasyonlu erişim sırasında değişmemelidir. |
| [Validation](./validation/) | Doğrulama sonucunu alırken mümkün olan optimizasyonu uygula. Doğrulamanın sonucunu etkileyebilecek tüm veri ve ayarlar (doğrulama ayarları, bağımlı hücre değerleri vb.) optimizasyonlu erişim sırasında değişmemelidir. |
