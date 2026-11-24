---
title: "PivotTable.PivotTableStyleType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Ruft den integrierten Pivot-Tabellenstil ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/pivottablestyletype/
---
## PivotTable.PivotTableStyleType property

Liest und legt den integrierten PivotTable-Stil fest.

```csharp
public PivotTableStyleType PivotTableStyleType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotTableStyleTypeDemo
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
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Pivot-Tabelle erstellen
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Setzen und demonstrieren Sie PivotTableStyleType
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            Console.WriteLine("PivotTable Style Type: " + pivotTable.PivotTableStyleType);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableStyleTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotTableStyleType](../../pivottablestyletype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


