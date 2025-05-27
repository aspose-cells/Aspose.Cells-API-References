---
title: Class SmartTagProperty
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Markup.SmartTagProperty class. Represents the property of the cell smart tag
type: docs
url: /net/aspose.cells.markup/smarttagproperty/
---
## SmartTagProperty class

Represents the property of the cell smart tag.

```csharp
public class SmartTagProperty
```

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.cells.markup/smarttagproperty/name/) { get; set; } | Gets and sets the name of the property. |
| [Value](../../aspose.cells.markup/smarttagproperty/value/) { get; set; } | Gets and sets the value of the property. |

### Examples

```csharp
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyDemo
    {
        public static void RunDemo()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            // Access the SmartTagSetting of the worksheet
            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;

            // Add a smart tag to cell A1
            int smartTagIndex = smartTagSetting.Add(0, 0); // A1 is at row 0, column 0
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            // Add properties to the smart tag
            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            // Add properties to the smart tag
            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Description", "Aspose.Cells SmartTag");

            // Save the workbook
            workbook.Save("SmartTagPropertyDemo.xlsx");

            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


