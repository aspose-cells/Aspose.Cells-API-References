---
title: "ListColumn.Range"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumn egenskap. Hämtar intervallet för denna listkolumn"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/range/
---
## ListColumn.Range property

Hämtar intervallet för denna listkolumn.

```csharp
public Range Range { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att skapa ett listobjekt
            worksheet.Cells["A1"].PutValue("Column1");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }
            
            // Skapa ett listobjekt
            int idx = worksheet.ListObjects.Add(0, 0, 4, 0, true);
            ListObject listObj = worksheet.ListObjects[idx];
            
            // Hämta den första listkolumnen
            ListColumn listCol = listObj.ListColumns[0];
            
            // Åtkomst till intervallet för listkolumnen
            Aspose.Cells.Range range = listCol.Range;
            
            // Visa intervallsinformation
            Console.WriteLine("Range address: " + range.Address);
            Console.WriteLine("Row count: " + range.RowCount);
            Console.WriteLine("Column count: " + range.ColumnCount);
            
            // Ändra celler i intervallet
            for (int i = 0; i < range.RowCount; i++)
            {
                range[i, 0].PutValue("Modified " + (i + 1));
            }
            
            // Spara arbetsboken
            workbook.Save("ListColumnRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


