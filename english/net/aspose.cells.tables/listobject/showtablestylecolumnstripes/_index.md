---
title: ListObject.ShowTableStyleColumnStripes
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Indicates whether column stripe formatting is applied to
type: docs
url: /net/aspose.cells.tables/listobject/showtablestylecolumnstripes/
---
## ListObject.ShowTableStyleColumnStripes property

Indicates whether column stripe formatting is applied to.

```csharp
public bool ShowTableStyleColumnStripes { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleColumnStripesDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Create a list object and get the reference
            int listObjectIndex = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Set column stripes property
            listObject.ShowTableStyleColumnStripes = true;
            
            // Save the workbook
            workbook.Save("ListObjectWithColumnStripes.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with column stripes enabled.");
        }
    }
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


