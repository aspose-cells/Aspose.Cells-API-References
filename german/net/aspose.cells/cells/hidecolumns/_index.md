---
title: "Cells.HideColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Mehrere Spalten ausblenden"
type: docs
url: /de/net/aspose.cells/cells/hidecolumns/
---
## Cells.HideColumns method

Blendet mehrere Spalten aus.

```csharp
public void HideColumns(int column, int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex. |
| totalColumns | Int32 | Spaltennummer. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnsWithInt32Int32Demo
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
                for (int j = 0; j < 10; j++)
                {
                    cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Spalten 3 bis 5 ausblenden (nullbasierter Index)
            int startColumn = 2; // Column C
            int columnCount = 3;  // Hide 3 columns
            cells.HideColumns(startColumn, columnCount);

            // Speichere die Arbeitsmappe
            workbook.Save("HideColumnsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


