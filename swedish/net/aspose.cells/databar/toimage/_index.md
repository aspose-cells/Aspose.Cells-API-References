---
title: "DataBar.ToImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataBar-metod. Rendera datastapel i cell till bildbytearray"
type: docs
url: /sv/net/aspose.cells/databar/toimage/
---
## DataBar.ToImage method

Rendera data bar i cell till bildbytearray.

```csharp
public byte[] ToImage(Cell cell, ImageOrPrintOptions imgOpts)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | Cell | Ange datastapeln i vilken cell som ska renderas |
| imgOpts | ImageOrPrintOptions | ImageOrPrintOptions innehåller vissa egenskaper för utdatabild |

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och villkorsstyrd formatering
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            
            // Lägg till villkorlig formatering för datastaplar
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
            
            // Hämta cellen med villkorsstyrd formatering
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult result = cell.GetConditionalFormattingResult();
            
            if (result != null && result.ConditionalFormattingDataBar != null)
            {
                DataBar bar = result.ConditionalFormattingDataBar;
                ImageOrPrintOptions imgOpts = new ImageOrPrintOptions();
                
                // Konvertera datastapel till bild
                byte[] img = bar.ToImage(cell, imgOpts);
                
                // Spara bilden
                string outputPath = "DataBarImage.png";
                File.WriteAllBytes(outputPath, img);
                
                // För bildverifiering måste du lägga till paketet System.Drawing.Common
                // och använd System.Drawing.Image om det behövs
                Console.WriteLine($"Data bar image saved to {outputPath}");
            }
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


