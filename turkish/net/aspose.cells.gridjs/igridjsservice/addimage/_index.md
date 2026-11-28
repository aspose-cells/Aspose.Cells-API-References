---
title: "IGridJsService.AddImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IGridJsService yöntemi. Görüntü baytlarını doğrudan alarak yerel dosyadan görüntü ekleme işlemini uygular"
type: docs
url: /tr/net/aspose.cells.gridjs/igridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

Yerel dosyadan resim ekleme işlemini uygular, resim baytlarını doğrudan alır.

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

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

Yerel dosyadan resim ekleme işlemini uygular, yüklenen form dosyalarını alır.

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

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


