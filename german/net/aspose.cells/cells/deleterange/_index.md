---
title: "Cells.DeleteRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Löscht einen Zellbereich und verschiebt Zellen gemäß der Verschiebungsoption"
type: docs
url: /de/net/aspose.cells/cells/deleterange/
---
## Cells.DeleteRange method

Löscht einen Zellbereich und verschiebt Zellen gemäß der Verschiebungsoption.

```csharp
public void DeleteRange(int startRow, int startColumn, int endRow, int endColumn, 
    ShiftType shiftType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Startzeilenindex. |
| startColumn | Int32 | Startspaltenindex. |
| endRow | Int32 | Endzeilenindex. |
| endColumn | Int32 | Endspaltenindex. |
| shiftType | ShiftType | Verschiebe‑Zellen‑Option. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRangeWithInt32Int32Int32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Einige Beispieldaten einfügen
            sheet.Cells["A1"].PutValue("A1");
            sheet.Cells["B1"].PutValue("B1");
            sheet.Cells["C1"].PutValue("C1");
            sheet.Cells["A2"].PutValue("A2");
            sheet.Cells["B2"].PutValue("B2");
            sheet.Cells["C2"].PutValue("C2");

            // Bereich löschen und nach links verschieben
            sheet.Cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);

            // Speichere die Arbeitsmappe
            workbook.Save("DeleteRangeExample.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


