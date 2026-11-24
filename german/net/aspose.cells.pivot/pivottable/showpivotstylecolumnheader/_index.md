---
title: "PivotTable.ShowPivotStyleColumnHeader"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob die Spaltenüberschrift in der Pivot-Tabelle den Stil erhalten soll"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showpivotstylecolumnheader/
---
## PivotTable.ShowPivotStyleColumnHeader property

Gibt an, ob die Spaltenüberschrift in der Pivot-Tabelle den Stil erhalten soll.

```csharp
public bool ShowPivotStyleColumnHeader { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleColumnHeaderDemo
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
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Fügen Sie eine Pivot-Tabelle hinzu
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // PivotTable konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // PivotTable-Stil festlegen
            pivotTable.ShowPivotStyleColumnHeader = true;
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableShowPivotStyleColumnHeaderDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


