---
title: "PivotTable.CalculateRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Berechnet den Bereich der Pivot-Tabellen"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/calculaterange/
---
## PivotTable.CalculateRange method

Berechnet den Bereich der PivotTable.

```csharp
public void CalculateRange()
```

### Hinweise

Wenn diese Methode nicht aufgerufen wurde, ist der Pivot-Tabellen-Bereich möglicherweise nicht korrekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge Beispieldaten zum ersten Arbeitsblatt hinzu
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Banana");
            dataSheet.Cells["B3"].PutValue(2000);
            dataSheet.Cells["A4"].PutValue("Orange");
            dataSheet.Cells["B4"].PutValue(3000);

            // Fügen Sie eine Pivot-Tabelle hinzu
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("A1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Zeilen- und Datenfelder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Bereich berechnen und Daten aktualisieren
            pivotTable.CalculateRange();
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableCalculateRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


