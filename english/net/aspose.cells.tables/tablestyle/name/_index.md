---
title: TableStyle.Name
second_title: Aspose.Cells for .NET API Reference
description: TableStyle property. Gets the name of table style
type: docs
url: /net/aspose.cells.tables/tablestyle/name/
---
## TableStyle.Name property

Gets the name of table style.

```csharp
public string Name { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.TableStylePropertyNameDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStylePropertyNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate sample data for table creation
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Employee");
            cells["B1"].PutValue("Department");
            cells["A2"].PutValue("John Doe");
            cells["B2"].PutValue("Engineering");
            cells["A3"].PutValue("Jane Smith");
            cells["B3"].PutValue("Marketing");

            // Create a table from the data range
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Display initial table style name
            Console.WriteLine("Initial table style: " + table.TableStyleName);

            // Apply a different built-in table style
            table.TableStyleType = TableStyleType.TableStyleDark1;

            // Display updated table style name and show style change impact
            Console.WriteLine("Applied table style: " + table.TableStyleName);

            // Save modified workbook with visible style changes
            workbook.Save("TableStyleNameDemo.xlsx");
        }
    }
}
```

### See Also

* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


