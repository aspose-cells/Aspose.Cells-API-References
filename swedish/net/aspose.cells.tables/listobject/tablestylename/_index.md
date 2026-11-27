---
title: "ListObject.TableStyleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject‑egenskap. Hämtar och anger tabellens stilnamn"
type: docs
url: /sv/net/aspose.cells.tables/listobject/tablestylename/
---
## ListObject.TableStyleName property

Hämtar och anger tabellens stilnamn.

```csharp
public string TableStyleName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa ett listobjekt/tabell
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Ange och visa tabellstilen
            table.TableStyleName = "TableStyleLight15";
            Console.WriteLine("Table style name: " + table.TableStyleName);

            // Spara arbetsboken
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


