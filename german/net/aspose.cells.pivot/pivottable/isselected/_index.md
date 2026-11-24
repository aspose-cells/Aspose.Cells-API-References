---
title: "PivotTable.IsSelected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob diese PivotTable ausgewählt ist"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/isselected/
---
## PivotTable.IsSelected property

Gibt an, ob diese PivotTable ausgewählt ist.

```csharp
public bool IsSelected { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsSelectedDemo
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
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

            // Zunächst ist IsSelected false
            Console.WriteLine("PivotTable IsSelected initially: " + pivotTable.IsSelected);

            // Wählen Sie die Pivot-Tabelle
            pivotTable.IsSelected = true;
            Console.WriteLine("PivotTable IsSelected after setting to true: " + pivotTable.IsSelected);

            // Die Auswahl der Pivot-Tabelle aufheben
            pivotTable.IsSelected = false;
            Console.WriteLine("PivotTable IsSelected after setting to false: " + pivotTable.IsSelected);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


