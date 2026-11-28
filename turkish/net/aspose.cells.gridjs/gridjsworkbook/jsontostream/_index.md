---
title: "GridJsWorkbook.JsonToStream"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridJsWorkbook yöntemi. Bellek içindeki Workbook'tan JSON üretir ve belirtilen akıma yazar. İsteğe bağlı olarak, üretilen JSON'u daha hızlı sonraki alımlar için önbelleğe alır. JsonToStreamByUid ile temel farklar: Bu yöntem, mevcut bellek içi Workbook durumu wb alanını kullanır. JsonToStreamByUid, Workbook'u diskteki .cells önbellek dosyalarından yeniden yükler. Değişikliklerden sonra mevcut workbook durumunu dışa aktarmak istediğinizde bu yöntemi kullanın. Önceden önbelleğe alınmış bir dosya durumundan JSON'u yeniden oluşturmanız gerektiğinde JsonToStreamByUid'yi kullanın. uid sağlandığında önbellekleme davranışı: JSON önbelleğini oluşturma öncesi L1 bellek ve L2 disk üzerinde kontrol eder. Önbellek yoksa, JSON'u bellek içi workbook'tan oluşturur. Oluşturulan JSON gelecekteki istekler için önbellekte saklanır."
type: docs
url: /tr/net/aspose.cells.gridjs/gridjsworkbook/jsontostream/
---
## GridJsWorkbook.JsonToStream method

Bellekteki Workbook'tan JSON oluşturur ve belirtilen akıma yazar. İsteğe bağlı olarak, oluşturulan JSON daha hızlı sonraki alımlar için önbelleğe alınır. JsonToStreamByUid ile temel farklar: - Bu yöntem mevcut bellek içi Workbook durumunu (wb alanı) kullanır - JsonToStreamByUid, Workbook'u disk üzerindeki .cells önbellek dosyalarından yeniden yükler - Değişikliklerden sonra mevcut çalışma kitabı durumunu dışa aktarmak istediğinizde bu yöntemi kullanın - Önceden önbelleğe alınmış bir dosya durumundan JSON yeniden oluşturmanız gerektiğinde JsonToStreamByUid'yi kullanın. Önbellekleme davranışı (uid sağlandığında): - Oluşturma öncesi JSON önbelleği kontrol eder (L1 bellek + L2 disk) - Önbellek yoksa, bellek içi workbook'tan JSON oluşturur - Oluşturulan JSON gelecekteki istekler için önbelleğe kaydedilir

```csharp
public void JsonToStream(Stream stream, string filename, string uid = null)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | JSON verisinin yazılacağı çıktı akışı |
| dosya adı | String | JSON içinde dosya adını belirtir. Null olarak ayarlanırsa, varsayılan dosya adı: book1. |
| uid | String | JSON önbelleklemesi için isteğe bağlı benzersiz tanımlayıcı. Sağlandığında, önbellek sorgulama ve depolamayı etkinleştirir. |

### Ayrıca Bakınız

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


