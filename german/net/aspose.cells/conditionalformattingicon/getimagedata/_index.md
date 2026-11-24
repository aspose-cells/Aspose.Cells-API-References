---
title: "ConditionalFormattingIcon.GetImageData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingIcon-Methode. Ruft die Bilddaten mit der Einstellung der Zelle ab"
type: docs
url: /de/net/aspose.cells/conditionalformattingicon/getimagedata/
---
## ConditionalFormattingIcon.GetImageData method

Liefert die Bilddaten mit den Zelleinstellungen.

```csharp
public byte[] GetImageData(Cell cell)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zelle | Zelle | Die Einstellung der Zelle. |

### Rückgabewert

Gibt die Bilddaten des Symbols zurück.

### Beispiele

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

### Siehe auch

* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


