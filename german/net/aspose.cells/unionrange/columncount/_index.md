---
title: "UnionRange.ColumnCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Eigenschaft. Gibt die Anzahl der Zeilen im Bereich zurück"
type: docs
url: /de/net/aspose.cells/unionrange/columncount/
---
## UnionRange.ColumnCount property

Liefert die Anzahl der Zeilen im Bereich.

```csharp
public int ColumnCount { get; }
```

### Hinweise

Nur wirksam, wenn es nur einen Bereich enthält.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = 1200;
            worksheet.Cells["C2"].Value = 5;
            worksheet.Cells["A3"].Value = "Phone";
            worksheet.Cells["B3"].Value = 800;
            worksheet.Cells["C3"].Value = 10;

            try
            {
                // Erstellen Sie Bereiche und kombinieren Sie sie zu einem Union-Bereich
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C2");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A3:C3");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // Zeige den Wert der ColumnCount-Eigenschaft an
                Console.WriteLine("ColumnCount of union range: " + unionRange.ColumnCount);

                // Demonstriere die Verwendung, indem du Spalteninformationen anzeigst
                Console.WriteLine("First column index: " + unionRange.FirstColumn);
                Console.WriteLine("Last column index: " + (unionRange.FirstColumn + unionRange.ColumnCount - 1));

                // Erstelle einen weiteren UnionRange mit unterschiedlicher Spaltenanzahl
                Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A1:B2");
                Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("D1:E2");
                UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

                // Vergleiche die Spaltenanzahlen
                Console.WriteLine("Second union range ColumnCount: " + unionRange2.ColumnCount);
                Console.WriteLine("First union range has " +
                    (unionRange.ColumnCount > unionRange2.ColumnCount ? "more" : "fewer") +
                    " columns than second union range");

                // Speichere die Arbeitsmappe
                workbook.Save("UnionRangeColumnCountDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


