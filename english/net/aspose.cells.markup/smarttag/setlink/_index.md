---
title: SmartTag.SetLink
second_title: Aspose.Cells for .NET API Reference
description: SmartTag method. Change the name and the namespace URI of the smart tag
type: docs
url: /net/aspose.cells.markup/smarttag/setlink/
---
## SmartTag.SetLink method

Change the name and the namespace URI of the smart tag.

```csharp
public void SetLink(string uri, string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| uri | String | The namespace URI of the smart tag. |
| name | String | The name of the smart tag. |

### Examples

```csharp
// Called: smartTag.SetLink("http://www.aspose.com", "AsposeLink");
public static void SmartTag_Method_SetLink()
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

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


