---
title: "ListObject.DisplayName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject egenskap. Hämtar och anger visningsnamnet för tabellen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/displayname/
---
## ListObject.DisplayName property

Hämtar och anger visningsnamnet för tabellen.

```csharp
public string DisplayName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Ange visningsnamn och demonstrera dess användning
            listObject.DisplayName = "ProductTable";
            Console.WriteLine("List Object Display Name: " + listObject.DisplayName);

            // Spara arbetsboken
            workbook.Save("ListObjectDisplayNameDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


