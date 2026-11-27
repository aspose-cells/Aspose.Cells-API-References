---
title: "ListColumn.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumn egenskap. Hämtar och anger namnet på kolumnen"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

Hämtar och anger namnet på kolumnen.

```csharp
public string Name { get; set; }
```

### Anmärkningar

Om namn på kolumnen sätts, kommer motsvarande cellvärde också att ändras.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Value");
            
            // Skapa ett tabell/list-objekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            Aspose.Cells.Tables.ListObject listObject = worksheet.ListObjects[index];

            // Åtkomst och ändring av Name-egenskapen för den första listkolumnen
            listObject.ListColumns[0].Name = "NewID";
            
            // Verifiera att namnet har satts
            Console.WriteLine("First column name: " + listObject.ListColumns[0].Name);
            
            // Spara arbetsboken
            workbook.Save("ListColumnPropertyNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


