---
title: "PivotTable.RowFields"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt eine PivotFieldCollection zurück, die derzeit als Zeilenfelder angezeigt wird"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/rowfields/
---
## PivotTable.RowFields property

Gibt eine [`PivotFieldCollection`](../../pivotfieldcollection/) zurück, die derzeit als Zeilenfelder angezeigt wird.

```csharp
public PivotFieldCollection RowFields { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowFieldsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bike";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Bike";
            cells["B3"].Value = "South";
            cells["C3"].Value = 800;
            
            cells["A4"].Value = "Car";
            cells["B4"].Value = "North";
            cells["C4"].Value = 1500;
            
            cells["A5"].Value = "Car";
            cells["B5"].Value = "South";
            cells["C5"].Value = 1200;

            // Pivot-Tabelle erstellen
            int pivotIndex = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Zeilenfelder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Demonstriere die RowFields-Eigenschaft
            Console.WriteLine("Row Fields Count: " + pivotTable.RowFields.Count);
            Console.WriteLine("First Row Field Name: " + pivotTable.RowFields[0].Name);
            Console.WriteLine("Second Row Field Name: " + pivotTable.RowFields[1].Name);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableRowFieldsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


