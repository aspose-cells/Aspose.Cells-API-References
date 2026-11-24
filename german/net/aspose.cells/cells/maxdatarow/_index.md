---
title: "Cells.MaxDataRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Maximaler Zeilenindex einer Zelle, die Daten enthält"
type: docs
url: /de/net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

Maximaler Zeilenindex der Zelle, die Daten enthält.

```csharp
public int MaxDataRow { get; }
```

### Hinweise

Gibt -1 zurück, wenn keine Zelle Daten enthält. Diese Eigenschaft muss Zellen und Zeilen dynamisch durchlaufen und prüfen, daher ist sie zeitaufwendig und sollte nicht wiederholt aufgerufen werden, etwa indem sie direkt als Bedingung in einer Schleife verwendet wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue(30);

            // Demonstrieren Sie die Verwendung von MaxDataRow
            int maxRow = sheet.Cells.MaxDataRow;
            Console.WriteLine("Max data row: " + maxRow);

            // Erstellen Sie einen Zellbereich mit MaxDataRow
            int startRow = 0;
            int startColumn = 0;
            int endRow = sheet.Cells.MaxDataRow;
            int endColumn = sheet.Cells.MaxDataColumn;

            // Formatierung auf den Datenbereich anwenden
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            
            // Stil auf den Bereich anwenden
            sheet.Cells.CreateRange(startRow, startColumn, endRow + 1, endColumn + 1).ApplyStyle(style, new StyleFlag { FontBold = true });

            // Speichere die Arbeitsmappe
            workbook.Save("MaxDataRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


