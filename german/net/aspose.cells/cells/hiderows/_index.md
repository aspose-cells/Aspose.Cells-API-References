---
title: "Cells.HideRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Versteckt mehrere Zeilen"
type: docs
url: /de/net/aspose.cells/cells/hiderows/
---
## Cells.HideRows method

Blendet mehrere Zeilen aus.

```csharp
public void HideRows(int row, int totalRows)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| totalRows | Int32 | Die Zeilennummer. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten befüllen
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i+1}, Col {j+1}";
                }
            }

            // Verstecke Zeilen 3 bis 5 (nullbasierter Index: 2 bis 4)
            worksheet.Cells.HideRows(2, 3);

            // Speichere die Arbeitsmappe
            workbook.Save("HideRowsExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


