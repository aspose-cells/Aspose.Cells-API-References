---
title: "Row.IsHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Row. Indica se la riga è nascosta"
type: docs
url: /it/net/aspose.cells/row/ishidden/
---
## Row.IsHidden property

Indica se la riga è nascosta.

```csharp
public bool IsHidden { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                cells[$"A{i + 1}"].PutValue($"Row {i + 1}");
            }

            // Nascondi alcune righe
            cells.HideRow(2);  // Row 3 (0-based index 2)
            cells.HideRow(5);  // Row 6 (0-based index 5)
            cells.HideRow(8);  // Row 9 (0-based index 8)

            // Verifica e visualizza lo stato IsHidden per ogni riga
            for (int i = 0; i < 10; i++)
            {
                bool isHidden = cells.Rows[i].IsHidden;
                Console.WriteLine($"Row {i + 1} is hidden: {isHidden}");
            }

            // Salva la cartella di lavoro
            workbook.Save("RowHiddenDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


