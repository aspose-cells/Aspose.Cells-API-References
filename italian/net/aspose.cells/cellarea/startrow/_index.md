---
title: "CellArea.StartRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Campo CellArea. Ottiene o imposta la riga iniziale di quest'area"
type: docs
url: /it/net/aspose.cells/cellarea/startrow/
---
## CellArea.StartRow field

Ottiene o imposta la riga iniziale di quest'area.

```csharp
public int StartRow;
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due oggetti CellArea
            CellArea area1 = new CellArea();
            area1.StartRow = 2;
            area1.StartColumn = 1;
            area1.EndRow = 5;
            area1.EndColumn = 3;

            CellArea area2 = new CellArea();
            area2.StartRow = area1.StartRow; // Demonstrating StartRow usage
            area2.StartColumn = area1.StartColumn;
            area2.EndRow = area1.EndRow;
            area2.EndColumn = area1.EndColumn;

            // Verifica che le aree corrispondano
            if (area1.StartRow == area2.StartRow &&
                area1.StartColumn == area2.StartColumn &&
                area1.EndRow == area2.EndRow &&
                area1.EndColumn == area2.EndColumn)
            {
                Console.WriteLine("CellArea objects match successfully");
                Console.WriteLine($"StartRow: {area1.StartRow}");
            }
            else
            {
                Console.WriteLine("CellArea objects do not match");
            }
        }
    }
}
```

### Vedi anche

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


