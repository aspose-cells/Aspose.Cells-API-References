---
title: "PivotTable.DataBodyRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Datenbereich in der Liste zwischen der Kopfzeilenzeile und der Einfügezeile enthält. Nur lesbar"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/databodyrange/
---
## PivotTable.DataBodyRange property

Gibt ein [`CellArea`](../../../aspose.cells/cellarea/) Objekt zurück, das den Bereich darstellt, der den Datenbereich in der Liste zwischen der Kopfzeilenzeile und der Einfügezeile enthält. Nur lesbar.

```csharp
public CellArea DataBodyRange { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataBodyRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 2500;

            // PivotTable hinzufügen
            int pivotIndex = sheet.PivotTables.Add("A7", "A1:B5", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // PivotTable konfigurieren
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot-Tabellendaten aktualisieren
            pivot.RefreshData();
            pivot.CalculateData();

            // Demonstriere die Verwendung von DataBodyRange
            CellArea dataBodyArea = pivot.DataBodyRange;
            Console.WriteLine($"Data body range: StartRow={dataBodyArea.StartRow}, EndRow={dataBodyArea.EndRow}, StartColumn={dataBodyArea.StartColumn}, EndColumn={dataBodyArea.EndColumn}");

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableDataBodyRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


