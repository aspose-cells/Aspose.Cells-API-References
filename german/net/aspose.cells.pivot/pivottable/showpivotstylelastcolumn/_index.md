---
title: "PivotTable.ShowPivotStyleLastColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob die Spaltenformatierung angewendet wird"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/showpivotstylelastcolumn/
---
## PivotTable.ShowPivotStyleLastColumn property

Gibt an, ob die Spaltenformatierung angewendet wird.

```csharp
public bool ShowPivotStyleLastColumn { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleLastColumnDemo
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

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // PivotTable-Stil festlegen und Stil für die letzte Spalte anzeigen
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;
            pivotTable.ShowPivotStyleLastColumn = true;

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableShowLastColumnStyle.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


