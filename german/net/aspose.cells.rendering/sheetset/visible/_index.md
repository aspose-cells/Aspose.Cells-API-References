---
title: "SheetSet.Visible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetSet-Eigenschaft. Gibt ein Set mit sichtbaren Blättern der Arbeitsmappe in ihrer ursprünglichen Reihenfolge zurück"
type: docs
url: /de/net/aspose.cells.rendering/sheetset/visible/
---
## SheetSet.Visible property

Erhält ein Set mit sichtbaren Blättern der Arbeitsmappe in ihrer ursprünglichen Reihenfolge.

```csharp
public static SheetSet Visible { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyVisibleDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit zwei Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Das zweite Arbeitsblatt ausblenden
            workbook.Worksheets[1].IsVisible = false;

            // Speicheroptionen einrichten, um nur sichtbare Blätter zu exportieren
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                SheetSet = SheetSet.Visible
            };

            // Arbeitsmappe speichern (nur sichtbares Blatt wird exportiert)
            workbook.Save("VisibleSheetsOnly.pptx", saveOptions);

            Console.WriteLine("Workbook saved with only visible sheets exported.");
        }
    }
}
```

### Siehe auch

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


