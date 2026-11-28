---
title: "DataBar.ToImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataBar yöntemi. Hücredeki veri çubuğunu görüntü bayt dizisine render edin"
type: docs
url: /tr/net/aspose.cells/databar/toimage/
---
## DataBar.ToImage method

Veri çubuğunu hücrede görüntü bayt dizisine dönüştürür.

```csharp
public byte[] ToImage(Cell cell, ImageOrPrintOptions imgOpts)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hücre | Hücre | Render edilecek hücredeki veri çubuğunu belirtin |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions, çıktı görüntüsünün bazı özelliklerini içerir |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class DataBarMethodToImageWithCellImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ve koşullu biçimlendirme ekle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            
            // Veri çubuğu koşullu biçimlendirmesi ekle
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);
            
            idx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcc[idx];
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            
            // Koşullu biçimlendirmeli hücreyi alın
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            if (result != null && result.ConditionalFormattingDataBar != null)
            {
                DataBar bar = result.ConditionalFormattingDataBar;
                ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
                
                // Veri çubuğunu görüntüye dönüştürün
                byte[] img = bar.ToImage(cell, imgOpts);
                
                // Görüntüyü kaydedin
                string outputPath = "DataBarImage.png";
                File.WriteAllBytes(outputPath, img);
                
                // Görüntü doğrulaması için System.Drawing.Common paketini eklemeniz gerekir
                // ve gerekirse System.Drawing.Image'ı kullanın
                Console.WriteLine($"Data bar image saved to {outputPath}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


