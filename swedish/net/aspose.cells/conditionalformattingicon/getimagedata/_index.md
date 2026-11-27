---
title: "ConditionalFormattingIcon.GetImageData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingIcon-metoden. Hämtar bilddata med cellens inställning"
type: docs
url: /sv/net/aspose.cells/conditionalformattingicon/getimagedata/
---
## ConditionalFormattingIcon.GetImageData method

Hämtar bilddata med cellens inställning.

```csharp
public byte[] GetImageData(Cell cell)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | Cell | Cellens inställning. |

### Returvärde

Returnerar bilddata för ikonen.

### Exempel

```csharp
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconMethodGetImageDataWithCellDemo
    {
        public static void Run()
        {
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            Workbook workbook = new Workbook("example.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingIcon icon = worksheet.ConditionalFormattings[0][0].IconSet.CfIcons[0];
            
            Cell targetCell = worksheet.Cells["E1"];
            byte[] imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "E1_icon.png"), imageData);
            
            targetCell = worksheet.Cells["G1"];
            imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "G1_icon.png"), imageData);
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


