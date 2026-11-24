---
title: "Cells.HideColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Versteckt eine Spalte"
type: docs
url: /de/net/aspose.cells/cells/hidecolumn/
---
## Cells.HideColumn method

Blendet eine Spalte aus.

```csharp
public void HideColumn(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setzen Sie einige Daten in die Spalte, die wir ausblenden
            cells["B1"].PutValue("This column will be hidden");
            cells["B2"].PutValue(123.45);

            // Spalte B ausblenden (Index 1)
            cells.HideColumn(1);

            // Spalte mit Standardbreite wieder einblenden
            cells.UnhideColumn(1, cells.StandardWidth);

            // Speichere die Arbeitsmappe
            workbook.Save("HideColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


