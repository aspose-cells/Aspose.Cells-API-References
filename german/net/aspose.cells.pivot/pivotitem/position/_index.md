---
title: "PivotItem.Position"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotItem-Eigenschaft. Gibt den Index dieses Elements in allen PivotItems des Feldes an"
type: docs
url: /de/net/aspose.cells.pivot/pivotitem/position/
---
## PivotItem.Position property

Angabe des Index dieses Elements in allen PivotItems des Feldes.

```csharp
public int Position { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyPositionDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Orange");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Demonstrieren Sie die Position-Eigenschaft
            PivotField rowField = pivotTable.RowFields[0];
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Before - Name: {item.Name}, Position: {item.Position}");
                item.Position = 0; // Set position to 0
                Console.WriteLine($"After - Name: {item.Name}, Position: {item.Position}");
            }

            // Pivot-Tabelle aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotItemPositionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


