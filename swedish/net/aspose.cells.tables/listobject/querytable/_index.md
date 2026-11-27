---
title: "ListObject.QueryTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject egenskap. Hämtar den länkade QueryTable"
type: docs
url: /sv/net/aspose.cells.tables/listobject/querytable/
---
## ListObject.QueryTable property

Hämtar den länkade QueryTable.

```csharp
public QueryTable QueryTable { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectPropertyQueryTableDemo
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

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            try
            {
                // Åtkomst till QueryTable-egenskapen (skrivskyddad)
                QueryTable queryTable = listObject.QueryTable;

                if (queryTable != null)
                {
                    // Visa QueryTable-egenskaper
                    Console.WriteLine("QueryTable Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Preserve Formatting: " + queryTable.PreserveFormatting);
                    Console.WriteLine("Adjust Column Width: " + queryTable.AdjustColumnWidth);

                    // Åtkomst till resultatrangen om den är tillgänglig
                    if (queryTable.ResultRange != null)
                    {
                        Console.WriteLine("Result Range Address: " + queryTable.ResultRange.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No QueryTable associated with this ListObject");
                }

                // Spara arbetsboken
                workbook.Save("QueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [QueryTable](../../../aspose.cells/querytable/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


