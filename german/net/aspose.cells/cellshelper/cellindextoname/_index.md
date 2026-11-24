---
title: "CellsHelper.CellIndexToName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Gibt den Zellenamen basierend auf Zeilen- und Spaltenindizes zurück"
type: docs
url: /de/net/aspose.cells/cellshelper/cellindextoname/
---
## CellsHelper.CellIndexToName method

Ermittelt den Zellnamen anhand seiner Zeilen- und Spaltenindizes.

```csharp
public static string CellIndexToName(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |
| column | Int32 | Spaltenindex. |

### Rückgabewert

Name der Zelle.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCellIndexToNameWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten befüllen
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);

            // Erhalte den Zellenamen aus Zeilen- und Spaltenindizes
            string cellName = CellsHelper.CellIndexToName(2, 1); // Row 2, Column 1 (B3)

            // Gib das Ergebnis aus
            Console.WriteLine("Cell name for row 2, column 1 is: " + cellName);
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


