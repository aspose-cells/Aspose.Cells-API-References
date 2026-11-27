---
title: "SaveOptions.UpdateSmartArt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Anger om uppdatering av SmartArt-inställning. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/saveoptions/updatesmartart/
---
## SaveOptions.UpdateSmartArt property

Anger om inställning för SmartArt ska uppdateras. Standardvärdet är falskt.

```csharp
public bool UpdateSmartArt { get; set; }
```

### Anmärkningar

Endast effekt efter att ha anropat metoden Shape.GetResultOfSmartArt() och de cachade formerna finns i mallfilen.

### Exempel

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
            // Läs in källarbetsboken
            Workbook workbook = new Workbook("example.xlsx");

            // Modifiera former och SmartArt
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

            // Spara med UpdateSmartArt aktiverat
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.UpdateSmartArt = true;
            workbook.Save("output.xlsx", saveOptions);

            // Verifiera ändringarna
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

### Se även

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


