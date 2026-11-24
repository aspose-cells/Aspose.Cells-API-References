---
title: "SaveOptions.UpdateSmartArt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SaveOptions-Eigenschaft. Gibt an, ob die SmartArt-Aktualisierungseinstellung aktiviert ist. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/saveoptions/updatesmartart/
---
## SaveOptions.UpdateSmartArt property

Gibt an, ob die SmartArt-Einstellung aktualisiert wird. Der Standardwert ist false.

```csharp
public bool UpdateSmartArt { get; set; }
```

### Hinweise

Wirkt nur nach Aufruf der Methode Shape.GetResultOfSmartArt() und wenn die zwischengespeicherten Formen in der Vorlagendatei vorhanden sind.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyUpdateSmartArtDemo
    {
        public static void Run()
        {
            // Lade die Quellarbeitsmappe
            Workbook workbook = new Workbook("example.xlsx");

            // Formen und SmartArt ändern
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    shape.AlternativeText = "ReplacedAlternativeText";
                    
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartArtShape in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            smartArtShape.Text = "ReplacedText";
                        }
                    }
                }
            }

            // Speichern mit aktivierter UpdateSmartArt
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.UpdateSmartArt = true;
            workbook.Save("output.xlsx", saveOptions);

            // Änderungen überprüfen
            Workbook savedWorkbook = new Workbook("output.xlsx");
            foreach (Worksheet worksheet in savedWorkbook.Worksheets)
            {
                foreach (Shape shape in worksheet.Shapes)
                {
                    Console.WriteLine($"Shape Alt Text: {shape.AlternativeText}");
                    
                    if (shape.IsSmartArt)
                    {
                        foreach (Shape smartArtShape in shape.GetResultOfSmartArt().GetGroupedShapes())
                        {
                            Console.WriteLine($"SmartArt Text: {smartArtShape.Text}");
                        }
                    }
                }
            }
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


