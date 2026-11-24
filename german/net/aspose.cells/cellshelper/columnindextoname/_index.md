---
title: "CellsHelper.ColumnIndexToName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Gibt den Spaltennamen gemäß Spaltenindex zurück"
type: docs
url: /de/net/aspose.cells/cellshelper/columnindextoname/
---
## CellsHelper.ColumnIndexToName method

Ermittelt den Spaltennamen anhand des Spaltenindex.

```csharp
public static string ColumnIndexToName(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex. |

### Rückgabewert

Name der Spalte.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnIndexToNameWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Werte in Zellen festlegen, um die Umwandlung von Spaltenindex zu Namen zu demonstrieren
            worksheet.Cells["A1"].PutValue("Column Index");
            worksheet.Cells["B1"].PutValue("Column Name");

            // Demonstriere ColumnIndexToName für Indizes 0‑4
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i);
                string columnName = CellsHelper.ColumnIndexToName(i);
                worksheet.Cells[i + 1, 1].PutValue(columnName);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ColumnIndexToNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


