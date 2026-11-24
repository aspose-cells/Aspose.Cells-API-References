---
title: "Cells.HideGroupDetail"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Klappt die gruppierten Zeilen/Spalten zusammen"
type: docs
url: /de/net/aspose.cells/cells/hidegroupdetail/
---
## Cells.HideGroupDetail method

Klappt die gruppierten Zeilen/Spalten zusammen.

```csharp
public void HideGroupDetail(bool isVertical, int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isVertical | Boolean | Wahr, klappe die gruppierten Zeilen zusammen. |
| Index | Int32 | Der Zeilen-/Spaltenindex |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gruppiere Zeilen und verberge Details
            worksheet.Cells.GroupRows(0, 9, false);
            worksheet.Cells.HideGroupDetail(true, 4);
            worksheet.Cells.HideGroupDetail(true, 7);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


