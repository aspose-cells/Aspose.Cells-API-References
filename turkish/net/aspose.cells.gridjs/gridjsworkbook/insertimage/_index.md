---
title: "GridJsWorkbook.InsertImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridJsWorkbook method. Görüntüyü dosya akışı veya URL'den çalışma sayfasına ekler; dosya akışı ya da URL sağlanmalıdır; p.type AutoShapeType'dan biri olduğunda şekil ekler."
type: docs
url: /tr/net/aspose.cells.gridjs/gridjsworkbook/insertimage/
---
## GridJsWorkbook.InsertImage method

Çalışma sayfasına dosya akışı veya URL'den (dosya akışı ya da URL sağlanmalıdır) görüntü ekler veya p.type AutoShapeType'tan biri olduğunda şekil ekler.

```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | String | Dosya önbelleği için benzersiz kimlik |
| p | String | İşlemin hücre konumunu, çalışma sayfası adını, görüntü için sol üst satırı, sol üst sütunu vb. belirten JSON biçim dizesi {name:'sheet1',ri:1,ci:1} |
| s | Stream | Görüntü dosyasının dosya akışı |
| imageUrl | String | Görüntü dosyasının URL'si |

### Dönüş Değeri

Eklenen görüntünün JSON biçim dizesi

### Ayrıca Bakınız

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


