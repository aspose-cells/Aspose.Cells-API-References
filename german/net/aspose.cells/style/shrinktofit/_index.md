---
title: "Style.ShrinkToFit"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen"
type: docs
url: /de/net/aspose.cells/style/shrinktofit/
---
## Style.ShrinkToFit property

Gibt an, ob der Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen.

```csharp
public bool ShrinkToFit { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // Ein Arbeitsmappenobjekt erstellen
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Auf die Cells-Sammlung zugreifen
            Cells cells = worksheet.Cells;
            
            // Setze etwas Text in Zelle A1, das länger ist als die Spaltenbreite
            cells["A1"].PutValue("This is a long text that needs shrinking to fit");
            
            // Setze die Spaltenbreite kleiner als die Textlänge
            cells.SetColumnWidth(0, 10);
            
            // Hole den Stil der Zelle A1
            Style style = cells["A1"].GetStyle();
            
            // Setze ShrinkToFit auf true
            style.ShrinkToFit = true;
            
            // Den Stil auf Zelle A1 anwenden
            cells["A1"].SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShrinkToFitDemo.xlsx");
            
            Console.WriteLine("ShrinkToFit demo completed successfully.");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


