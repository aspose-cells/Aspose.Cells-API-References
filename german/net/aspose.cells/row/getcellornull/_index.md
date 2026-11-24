---
title: "Row.GetCellOrNull"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Methode. Gibt die Zelle oder null am angegebenen Index zurück."
type: docs
url: /de/net/aspose.cells/row/getcellornull/
---
## Row.GetCellOrNull method

Gibt die Zelle oder null am angegebenen Index zurück.

```csharp
public Cell GetCellOrNull(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Der Spalten‑Index |

### Rückgabewert

Gibt das Zellenobjekt zurück, wenn die Zelle existiert. Oder gibt null zurück, wenn das Zellenobjekt nicht existiert.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellOrNullWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            ws.Cells["A1"].PutValue("Header1");
            ws.Cells["B1"].PutValue("Header2");
            ws.Cells["A2"].PutValue(100);
            ws.Cells["B2"].PutValue(200);

            // Rufen Sie die erste Zeile ab
            Row row = ws.Cells.Rows[0];

            // Demonstration von GetCellOrNull mit Int32‑Parameter
            for (int colIndex = 0; colIndex < 2; colIndex++)
            {
                Cell cell = row.GetCellOrNull(colIndex);
                if (cell != null)
                {
                    Console.WriteLine($"Cell at column {colIndex}: {cell.StringValue}");
                }
                else
                {
                    Console.WriteLine($"Cell at column {colIndex} is null");
                }
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


