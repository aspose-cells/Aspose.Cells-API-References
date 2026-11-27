---
title: "ListObject.DataRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject egenskap. Hämtar datarangen för tabellen"
type: docs
url: /sv/net/aspose.cells.tables/listobject/datarange/
---
## ListObject.DataRange property

Hämtar dataintervallet för tabellen.

```csharp
public Range DataRange { get; }
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDataRangeDemo
    {
        public static void Run()
        {
            Encoding.RegisterProvider(CodePagesEncodingProvider.Instance);
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Skapa ett ListObject (Tabell)
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "EmployeeTable";

            // Hämta datarangen för tabellen
            Aspose.Cells.Range dataRange = table.DataRange;

            // Demonstrera användning av DataRange
            Console.WriteLine("Table Data Range: " + dataRange.Address);
            Console.WriteLine("Row Count: " + dataRange.RowCount);
            Console.WriteLine("Column Count: " + dataRange.ColumnCount);

            // Lägg till en formel i sista kolumnen med hjälp av DataRange
            string formula = "=CONCATENATE(\"ID-\", [ID])";
            int lastColIndex = dataRange.ColumnCount - 1;
            dataRange[0, lastColIndex].PutValue("FormattedID");
            for (int i = 1; i < dataRange.RowCount; i++)
            {
                dataRange[i, lastColIndex].Formula = formula;
            }

            // Spara arbetsboken
            workbook.Save("ListObjectDataRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../../../aspose.cells/range/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


