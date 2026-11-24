---
title: "Cells.GroupRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gruppiert Zeilen"
type: docs
url: /de/net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

Gruppiert Zeilen.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | Int32 | Der Index der ersten Zeile, die gruppiert werden soll. |
| lastIndex | Int32 | Der Index der letzten Zeile, die gruppiert werden soll. |
| isHidden | Boolean | Gibt an, ob die gruppierten Zeilen ausgeblendet sind. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Einige Daten befüllen
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Group {i + 1}");
                for (int j = 1; j <= 5; j++)
                {
                    cells[i, j].PutValue($"Data {j}");
                }
            }

            // Gruppiere Zeilen 1 bis 5 (0-basierter Index) und blende sie aus
            cells.GroupRows(1, 5, true);

            // Setze Zusammenfassungszeile unter die Gruppe
            worksheet.Outline.SummaryRowBelow = false;

            // Speichere die Arbeitsmappe
            workbook.Save("GroupRowsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

Gruppiert Zeilen.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | Int32 | Der Index der ersten Zeile, die gruppiert werden soll. |
| lastIndex | Int32 | Der Index der letzten Zeile, die gruppiert werden soll. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Einige Beispieldaten einfügen
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Gruppiere Zeilen 2 bis 5 (0-basierter Index)
            cells.GroupRows(1, 4);

            // Speichere die Arbeitsmappe
            workbook.Save("GroupRowsExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


