---
title: "Row.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-egenskap. Hämtar cellen"
type: docs
url: /sv/net/aspose.cells/row/item/
---
## Row indexer

Hämtar cellen.

```csharp
public Cell this[int column] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| column | Kolumnindexet |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Få åtkomst till den första raden
            Row row = sheet.Cells.Rows[0];
            
            // Ställ in HTML-innehåll med olika färgstilar
            row[0].HtmlString = @"<span style=""color:#ffAb68;"">TEST</span>";
            row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
            
            // Demonstrera användning av Item-egenskapen och skriv ut färgerna
            Console.WriteLine("Cell 0 Font Color: " + row[0].GetStyle().Font.Color.Name);
            Console.WriteLine("Cell 1 Font Color: " + row[1].GetStyle().Font.Color.Name);
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


