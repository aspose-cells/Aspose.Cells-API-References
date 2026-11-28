---
title: "GridJsService.AddImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridJsService yöntemi. Yerel dosyadan resim ekleme işlemini uygular; dosya baytları JS FormData'dan veya herhangi bir host'tan gelir."
type: docs
url: /tr/net/aspose.cells.gridjs/gridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Yerel dosyadan resim ekleme işlemini uygular (dosya baytları JS FormData'dan veya herhangi bir ana bilgisayardan gelir).

```csharp
public string AddImage(string p, string uid, string iscontrol, byte[] fileBytes)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | String | JSON dize parametresi |
| uid | String | Dosya önbelleği için benzersiz kimlik. |
| iscontrol | String | Kontrol olup olmadığını belirtin. |
| fileBytes | Byte[] | Görüntü dosyasının ham baytları. |

### Dönüş Değeri

JSON dize sonucu

### Ayrıca Bakınız

* class [GridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Yerel dosyadan resim ekleme işlemini uygular.

```csharp
public string AddImage(string p, string uid, string iscontrol, IFormFileCollection files)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | String | JSON dize parametresi |
| uid | String | Dosya önbelleği için benzersiz kimlik. |
| iscontrol | String | Kontrol olup olmadığını belirtin. |
| dosyalar | IFormFileCollection | Görüntünün form dosyası. |

### Dönüş Değeri

JSON dize sonucu

### Ayrıca Bakınız

* class [GridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


