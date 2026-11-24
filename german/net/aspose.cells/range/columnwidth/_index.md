---
title: "Range.ColumnWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Setzt oder liest die Spaltenbreite dieses Bereichs"
type: docs
url: /de/net/aspose.cells/range/columnwidth/
---
## Range.ColumnWidth property

Setzt oder liefert die Spaltenbreite dieses Bereichs

```csharp
public double ColumnWidth { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyColumnWidthDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf einen Bereich (Spalten B bis D) zu
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B:D");
            
            // Zeige die aktuelle Spaltenbreite an
            Console.WriteLine("Current ColumnWidth: " + range.ColumnWidth);

            // Setze neue Spaltenbreite (in Zeicheneinheiten)
            range.ColumnWidth = 15.0;

            // Fülle Zellen, um die Wirkung zu demonstrieren
            worksheet.Cells["B1"].PutValue("This is column B");
            worksheet.Cells["C1"].PutValue("This is column C");
            worksheet.Cells["D1"].PutValue("This is column D");

            // Zeilen automatisch anpassen, um den Inhalt anzuzeigen
            worksheet.AutoFitRows();

            // Speichere die Arbeitsmappe
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


