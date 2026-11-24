---
title: "PivotTable.ColumnFields"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt ein PivotFields-Objekt zurück, das derzeit als Spaltenfelder angezeigt wird"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/columnfields/
---
## PivotTable.ColumnFields property

Gibt ein PivotFields-Objekt zurück, das derzeit als Spaltenfelder angezeigt wird.

```csharp
public PivotFieldCollection ColumnFields { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnFieldsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bikes";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Bikes";
            cells["B3"].Value = 200;
            cells["A4"].Value = "Cars";
            cells["B4"].Value = 300;
            cells["A5"].Value = "Cars";
            cells["B5"].Value = 400;
            cells["A6"].Value = "Trucks";
            cells["B6"].Value = 500;

            // PivotTable hinzufügen
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilen- und Spaltenfelder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Sales");

            // Auf das Spaltenfeld zugreifen und es manipulieren
            PivotField columnField = pivotTable.ColumnFields[0];
            columnField.FilterByValue(0, PivotFilterType.ValueGreaterThan, 300, 0);

            // Daten berechnen und aktualisieren
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableColumnFieldsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


