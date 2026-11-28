---
title: "Range.ToHtml"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Aralığı html'ye dönüştür"
type: docs
url: /tr/net/aspose.cells/range/tohtml/
---
## Range.ToHtml method

Aralığı html'ye dönüştür.

```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Aralığı html'ye dönüştürmek için seçenekler. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToHtmlWithHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1:J25 aralığına bazı veriler ekle
            for (int i = 0; i < 25; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Cell {i+1},{j+1}";
                }
            }

            // Tam nitelikli tip adıyla bir aralık oluştur
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:J25");
            
            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportImagesAsBase64 = true;
            
            // Aralığı HTML'ye dönüştür
            byte[] htmlData = range.ToHtml(options);
            
            // HTML'yi dosyaya kaydet
            File.WriteAllBytes("output.html", htmlData);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


