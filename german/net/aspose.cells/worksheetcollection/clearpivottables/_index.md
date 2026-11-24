---
title: "WorksheetCollection.ClearPivottables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Löscht Pivot-Tabellen aus der Kalkulationstabelle"
type: docs
url: /de/net/aspose.cells/worksheetcollection/clearpivottables/
---
## WorksheetCollection.ClearPivottables method

Löscht Pivot‑Tabellen aus dem Tabellenblatt.

```csharp
public void ClearPivottables()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodClearPivottablesDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für Pivot‑Tabelle erstellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Fügen Sie eine Pivot-Tabelle hinzu
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            Console.WriteLine("Pivot tables count before clearing: " + worksheet.PivotTables.Count);

            // Lösche alle Pivot-Tabellen aus allen Arbeitsblättern
            workbook.Worksheets.ClearPivottables();

            Console.WriteLine("Pivot tables count after clearing: " + worksheet.PivotTables.Count);
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


