---
title: Class SmartTag
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Markup.SmartTag class. Represents a smart tag
type: docs
url: /net/aspose.cells.markup/smarttag/
---
## SmartTag class

Represents a smart tag.

```csharp
public class SmartTag
```

## Properties

| Name | Description |
| --- | --- |
| [Deleted](../../aspose.cells.markup/smarttag/deleted/) { get; set; } | Indicates whether the smart tag is deleted. |
| [Name](../../aspose.cells.markup/smarttag/name/) { get; } | Gets the name of the smart tag. |
| [Properties](../../aspose.cells.markup/smarttag/properties/) { get; set; } | Gets and set the properties of the smart tag. |
| [Uri](../../aspose.cells.markup/smarttag/uri/) { get; } | Gets the namespace URI of the smart tag. |

## Methods

| Name | Description |
| --- | --- |
| [SetLink](../../aspose.cells.markup/smarttag/setlink/)(string, string) | Change the name and the namespace URI of the smart tag. |

### Examples

```csharp
// Called: SmartTag smartTag = smartTags[0];
public static void Type_SmartTag()
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
```

### See Also

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


