---
title: "ListObject.AutoFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject egenskap. Hämtar autofilter för den här tabellen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/autofilter/
---
## ListObject.AutoFilter property

Hämtar autofilter för den här tabellen.

```csharp
public AutoFilter AutoFilter { get; }
```

### Anmärkningar

Det fungerar endast när [`HasAutoFilter`](../hasautofilter/) är falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAutoFilterDemo
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
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Skapa ett ListObject
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Ändra storlek på listobjektet så att det inkluderar all data
            listObject.Resize(0, 0, 4, 2, true);

            // Kom åt och demonstrera AutoFilter-funktionalitet
            if (listObject.AutoFilter != null)
            {
                // Applicera filter på Ålder-kolumnen (kolumn 2)
                listObject.AutoFilter.Filter(1, "25");
                
                // Visa filtrerad data
                Console.WriteLine("Filtered Data:");
                for (int row = 1; row <= 4; row++)
                {
                    if (!worksheet.Cells.Rows[row].IsHidden)
                    {
                        Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                    }
                }

                // Rensa filtret
                listObject.AutoFilter.RemoveFilter(1);
            }

            // Spara arbetsboken
            workbook.Save("ListObjectAutoFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


