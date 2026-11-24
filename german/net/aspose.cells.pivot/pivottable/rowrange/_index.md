---
title: "PivotTable.RowRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Zeilenbereich im PivotTable-Bericht enthält. Nur lesbar"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/rowrange/
---
## PivotTable.RowRange property

Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Zeilenbereich im PivotTable-Bericht enthält. Nur lesbar.

```csharp
public CellArea RowRange { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowRangeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Aktualisiere alle PivotTables in der Arbeitsmappe.
            workbook.Worksheets.RefreshAll();
            
            // Hole die erste Pivot-Tabelle aus dem ersten Arbeitsblatt
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[0];
            
            // Hole den Zeilenbereich der Pivot-Tabelle
            CellArea rowRange = pivotTable.RowRange;
            
            // Zeige die Koordinaten des Zeilenbereichs an
            Console.WriteLine("PivotTable Row Range:");
            Console.WriteLine($"Start Row: {rowRange.StartRow}");
            Console.WriteLine($"End Row: {rowRange.EndRow}");
            Console.WriteLine($"Start Column: {rowRange.StartColumn}");
            Console.WriteLine($"End Column: {rowRange.EndColumn}");
            
            // Hole den Spaltenbereich der Pivot-Tabelle
            CellArea columnRange = pivotTable.ColumnRange;
            
            // Zeige die Koordinaten des Spaltenbereichs an
            Console.WriteLine("\nPivotTable Column Range:");
            Console.WriteLine($"Start Row: {columnRange.StartRow}");
            Console.WriteLine($"End Row: {columnRange.EndRow}");
            Console.WriteLine($"Start Column: {columnRange.StartColumn}");
            Console.WriteLine($"End Column: {columnRange.EndColumn}");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


