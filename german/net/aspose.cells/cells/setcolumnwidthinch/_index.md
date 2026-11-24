---
title: "Cells.SetColumnWidthInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Setzt die Spaltenbreite in Zoll im Normalansicht"
type: docs
url: /de/net/aspose.cells/cells/setcolumnwidthinch/
---
## Cells.SetColumnWidthInch method

Setzt die Spaltenbreite in Zoll in der Normalansicht.

```csharp
public void SetColumnWidthInch(int column, double inches)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex. |
| Zoll | Double | Anzahl der Zoll. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Spaltenbreiten in Zoll festlegen
            cells.SetColumnWidthInch(0, 2.0);
            cells.SetColumnWidthInch(1, 1.5);
            cells.SetColumnWidthInch(2, 0.8);

            // Einige Daten in Zellen setzen, um die Datei sichtbar zu machen
            cells["A1"].PutValue("Column A (2 inches)");
            cells["B1"].PutValue("Column B (1.5 inches)");
            cells["C1"].PutValue("Column C (0.8 inches)");

            // Speichere die Arbeitsmappe
            workbook.Save("ColumnWidthsInInches.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


