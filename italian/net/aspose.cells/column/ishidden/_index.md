---
title: "Column.IsHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Column. Indica se la colonna è nascosta"
type: docs
url: /it/net/aspose.cells/column/ishidden/
---
## Column.IsHidden property

Indica se la colonna è nascosta.

```csharp
public bool IsHidden { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta la larghezza della colonna per la dimostrazione
            worksheet.Cells.Columns[1].Width = 20;
            Console.WriteLine("Column 1 width before hiding: " + worksheet.Cells.Columns[1].Width);

            // Nascondi la colonna
            worksheet.Cells.Columns[1].IsHidden = true;
            Console.WriteLine("Column 1 is hidden: " + worksheet.Cells.Columns[1].IsHidden);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


