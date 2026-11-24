---
title: "PivotTable.ColumnRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable property. Gibt ein CellArea‑Objekt zurück, das den Bereich darstellt, der den Spaltenbereich im PivotTable‑Bericht enthält. Nur lesbar"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/columnrange/
---
## PivotTable.ColumnRange property

Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Spaltenbereich im PivotTable-Bericht enthält. Schreibgeschützt.

```csharp
public CellArea ColumnRange { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnRangeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;
            
            // Pivot-Tabelle erstellen
            int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Pivot-Tabellendaten aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spaltenbereich der Pivot-Tabelle abrufen
            CellArea columnRange = pivotTable.ColumnRange;
            Console.WriteLine("Pivot Table Column Range: " + columnRange);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableColumnRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


