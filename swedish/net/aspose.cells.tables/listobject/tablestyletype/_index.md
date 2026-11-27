---
title: "ListObject.TableStyleType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject-egenskap. Hämtar den inbyggda tabellstilen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/tablestyletype/
---
## ListObject.TableStyleType property

Hämtar och den inbyggda tabellstilen.

```csharp
public TableStyleType TableStyleType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i+1}-{j+1}");
                }
            }
            
            // Hämta samlingen av listobjekt
            ListObjectCollection tables = worksheet.ListObjects;
            
            // Lägg till en tabell
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[0];
            
            // Ställ in tabellstilen
            table.TableStyleType = TableStyleType.TableStyleDark2;
            
            // Spara arbetsboken
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TableStyleType](../../tablestyletype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


