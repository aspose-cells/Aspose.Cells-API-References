---
title: "Cells.IsRowHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Prüft, ob eine Zeile am angegebenen Index ausgeblendet ist"
type: docs
url: /de/net/aspose.cells/cells/isrowhidden/
---
## Cells.IsRowHidden method

Überprüft, ob eine Zeile am angegebenen Index ausgeblendet ist.

```csharp
public bool IsRowHidden(int rowIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Zeilenindex |

### Rückgabewert

wahr, wenn die Zeile ausgeblendet ist

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsRowHiddenWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Beispieldaten
            cells[1, 0].PutValue("US");
            cells[2, 0].PutValue("UK");
            cells[3, 0].PutValue("India");
            cells[4, 0].PutValue("UK");
            cells[5, 0].PutValue("India");
            cells[6, 0].PutValue("US");
            
            // Filter anwenden
            AutoFilter af = sheet.AutoFilter;
            af.Range = "A1:A1";
            af.Filter(0, "India");
            af.Refresh();
            
            // Zeilensichtbarkeit prüfen
            Console.WriteLine("Row Visibility Check:");
            for (int i = 1; i < 7; i++)
            {
                Console.WriteLine($"Row {i} hidden: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


