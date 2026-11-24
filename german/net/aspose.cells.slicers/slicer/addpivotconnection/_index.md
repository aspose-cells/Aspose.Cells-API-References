---
title: "Slicer.AddPivotConnection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Methode. Fügt eine PivotTable-Verbindung hinzu."
type: docs
url: /de/net/aspose.cells.slicers/slicer/addpivotconnection/
---
## Slicer.AddPivotConnection method

Fügt eine PivotTable‑Verbindung hinzu.

```csharp
public void AddPivotConnection(PivotTable pivot)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | Das PivotTable-Objekt |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerMethodAddPivotConnectionWithPivotTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Slicer hinzufügen – korrigierte Parameter
            int slicerIndex = sheet.Slicers.Add(pivotTable, 0, 0, "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Pivot-Verbindung zum Slicer hinzufügen
            slicer.AddPivotConnection(pivotTable);

            // Speichere die Arbeitsmappe
            workbook.Save("SlicerAddPivotConnectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


