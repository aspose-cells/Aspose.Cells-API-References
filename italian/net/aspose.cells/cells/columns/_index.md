---
title: "Cells.Columns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene la raccolta di oggetti Column che rappresentano le singole colonne in questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/columns/
---
## Cells.Columns property

Ottiene la raccolta di [`Column`](../../column/) oggetti che rappresentano le singole colonne in questo foglio di lavoro.

```csharp
public ColumnCollection Columns { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyColumnsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta lo stile per la colonna 5
            Style columnStyle = workbook.CreateStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 12;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { FontName = true, FontSize = true, FontBold = true });

            // Imposta la larghezza per la colonna 5
            cells.Columns[5].Width = 20;

            // Imposta i dati nella colonna 5 per dimostrare lo stile
            for (int row = 0; row < 10; row++)
            {
                cells[row, 5].PutValue($"Row {row + 1}");
            }

            // Salva la cartella di lavoro
            workbook.Save("ColumnsPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


