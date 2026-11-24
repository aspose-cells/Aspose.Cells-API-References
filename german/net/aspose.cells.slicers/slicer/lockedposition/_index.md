---
title: "Slicer.LockedPosition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer‑Eigenschaft. Gibt an, ob der angegebene Slicer über die Benutzeroberfläche verschoben oder in der Größe geändert werden kann"
type: docs
url: /de/net/aspose.cells.slicers/slicer/lockedposition/
---
## Slicer.LockedPosition property

Gibt an, ob der angegebene Slicer über die Benutzeroberfläche verschoben oder in der Größe geändert werden kann.

```csharp
public bool LockedPosition { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyLockedPositionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für die Pivot‑Tabelle hinzu
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Pivot‑Tabellensammlung erstellen
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Erstelle eine Pivot-Tabelle
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Zeilenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Datenfeld hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Slicer‑Sammlung erstellen
            SlicerCollection slicers = worksheet.Slicers;
            
            // Füge einen Slicer für die Pivot‑Tabelle hinzu
            int slicerIndex = slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = slicers[slicerIndex];

            // Slicer‑Eigenschaften festlegen
            slicer.Caption = "Fruit Slicer";
            slicer.NumberOfColumns = 2;
            slicer.WidthPixel = 200;
            slicer.HeightPixel = 150;

            // Demonstriere die LockedPosition‑Eigenschaft
            slicer.LockedPosition = true; // Lock the slicer position
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Ändern Sie die LockedPosition auf false, um Bewegung zu ermöglichen
            slicer.LockedPosition = false;
            Console.WriteLine("Slicer position locked: " + slicer.LockedPosition);

            // Speichere die Arbeitsmappe
            workbook.Save("SlicerLockedPositionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


