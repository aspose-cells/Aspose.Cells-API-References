---
title: "Row.IsCollapsed"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Row proprietà. Indica se la riga è compressa"
type: docs
url: /it/net/aspose.cells/row/iscollapsed/
---
## Row.IsCollapsed property

se la riga è compressa

```csharp
public bool IsCollapsed { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea e stila una riga
            Row row = worksheet.Cells.Rows[0];
            row.Height = 20;
            row.GroupLevel = 1;
            
            // Dimostra la proprietà IsCollapsed
            row.IsCollapsed = true;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Espandi la riga
            row.IsCollapsed = false;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Salva la cartella di lavoro
            workbook.Save("RowIsCollapsedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


