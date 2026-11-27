---
title: "ColumnCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ColumnCollection-egenskap. Hämtar ett Column-objekt efter kolumnindex. Column-objektet för det angivna kolumnindexet kommer att skapas om det inte redan finns."
type: docs
url: /sv/net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

Hämtar ett [`Column`](../../column/) objekt efter kolumnindex. Column-objektet för det angivna kolumnindexet kommer att skapas om det inte redan finns.

```csharp
public Column this[int columnIndex] { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till kolumnsamling
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Ställ in bredd för kolumner med Item-egenskapen
            columns[0].Width = 10;
            columns[1].Width = 15;
            columns[2].Width = 20;
            
            // Visa kolumnbredder
            Console.WriteLine("Column 0 Width: " + columns[0].Width);
            Console.WriteLine("Column 1 Width: " + columns[1].Width);
            Console.WriteLine("Column 2 Width: " + columns[2].Width);
            
            // Verifiera att kolumnbredderna är korrekt inställda
            if (columns[0].Width != 10 || columns[1].Width != 15 || columns[2].Width != 20)
            {
                throw new Exception("Column widths were not set correctly");
            }
        }
    }
}
```

### Se även

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


