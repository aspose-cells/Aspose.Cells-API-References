---
title: "GridPdfSaveOptions.SetImageResample"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GridPdfSaveOptions yöntemi. Yeniden örnekleme görüntülerinin istenen PPI (inç başına piksel) ve jpeg kalitesini ayarlar. Tüm görüntüler belirtilen kalite ayarıyla JPEG'e dönüştürülecek ve belirtilen PPI değerinden daha yüksek olan görüntüler yeniden örneklenmiş olacaktır"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/
---
## GridPdfSaveOptions.SetImageResample method

İstenen PPI (inç başına piksel) değerini yeniden örnekleme görüntüleri ve jpeg kalitesi için ayarlar. Tüm görüntüler belirtilen kalite ayarıyla JPEG'e dönüştürülecek ve belirtilen PPI (inç başına piksel) değerinden büyük olan görüntüler yeniden örneklenir.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| desiredPPI | Int32 | İnç başına istenen piksel. 220 yüksek kalite. 150 ekran kalitesi. 96 e-posta kalitesi. |
| jpegQuality | Int32 | 0 - %100 JPEG kalitesi. |

### Örnekler

Aşağıdaki kod, çıktı PDF'indeki görüntüler için istenen PPI'yi 96 ve jpeg kalitesini 80 olarak ayarlar.

```csharp
//kaynak dosyayı görüntülerle yükle.
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//istenen PPI'yi 96 ve jpeg kalitesini 80 olarak ayarla.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### Ayrıca Bakınız

* class [GridPdfSaveOptions](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


