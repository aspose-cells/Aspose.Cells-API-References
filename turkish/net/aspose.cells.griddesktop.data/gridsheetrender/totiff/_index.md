---
title: "GridSheetRender.ToTiff"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridSheetRender yöntemi. Tüm çalışma sayfasını Tiff Görüntüsü olarak akıma oluştur."
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridsheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Tüm çalışma sayfasını Tiff Image olarak akışa render et.

```csharp
public void ToTiff(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | çıktı görüntüsünün akışı |

### Ayrıca Bakınız

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToTiff(string) {#totiff_1}

Tüm çalışma sayfasını Tiff Image olarak bir dosyaya render et.

```csharp
public void ToTiff(string filename)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | String | çıktı görüntüsünün dosya adı |

### Örnekler

Aşağıdaki kod, ilk sayfanın tüm sayfalarını Tiff görüntüsü olarak çıkarır.

```csharp
//kaynak dosyayı görüntülerle yükle.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//Çıktı görüntü tipini ayarla.
imgOpt.SaveFormat = SaveFormat.Tiff;

//İlk sayfayı oluştur.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//Sayfanın tüm sayfalarını Tiff görüntüsüne çıkar.
sr.ToTiff("output.tiff");
```

### Ayrıca Bakınız

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


