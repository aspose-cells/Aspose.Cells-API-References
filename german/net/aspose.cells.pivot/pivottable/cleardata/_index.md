---
title: "PivotTable.ClearData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Daten und Formatierung der PivotTable-Ansicht löschen."
type: docs
url: /de/net/aspose.cells.pivot/pivottable/cleardata/
---
## PivotTable.ClearData method

Löscht Daten und Formatierung der PivotTable‑Ansicht.

```csharp
public void ClearData()
```

### Hinweise

Wenn diese Methode nicht aufgerufen wird, bevor Sie ein PivotField hinzufügen oder löschen, sind die PivotTable-Daten möglicherweise nicht korrekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodClearDataDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(15);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Felder zur Pivot-Tabelle hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("Pivot table with data:");
            Console.WriteLine(worksheet.Cells["D1"].StringValue);
            Console.WriteLine(worksheet.Cells["D2"].StringValue);
            Console.WriteLine(worksheet.Cells["D3"].StringValue);

            // PivotTable-Daten löschen
            pivotTable.ClearData();
            Console.WriteLine("\nAfter ClearData():");
            Console.WriteLine("Pivot table row count: " + (pivotTable.DataBodyRange.EndRow - pivotTable.DataBodyRange.StartRow + 1));

            // PivotTable neu erstellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nRebuilt pivot table:");
            Console.WriteLine(worksheet.Cells["D1"].StringValue);
            Console.WriteLine(worksheet.Cells["D2"].StringValue);
            Console.WriteLine(worksheet.Cells["D3"].StringValue);

            // Arbeitsmappe speichern.
            workbook.Save("PivotTableClearDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


