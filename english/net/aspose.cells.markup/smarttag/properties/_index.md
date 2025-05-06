---
title: SmartTag.Properties
second_title: Aspose.Cells for .NET API Reference
description: SmartTag property. Gets and set the properties of the smart tag
type: docs
url: /net/aspose.cells.markup/smarttag/properties/
---
## SmartTag.Properties property

Gets and set the properties of the smart tag.

```csharp
public SmartTagPropertyCollection Properties { get; set; }
```

### Examples

```csharp
// Called: SmartTagPropertyCollection properties = smartTag.Properties;
public static void Property_Properties()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Aspose&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;Cells&quot;);

            // Access the SmartTagSetting of the worksheet
            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;

            // Add a smart tag to cell A1
            int smartTagIndex = smartTagSetting.Add(0, 0); // A1 is at row 0, column 0
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            // Add properties to the smart tag
            smartTags.Add(&quot;http://docs.aspose.com&quot;, &quot;docs&quot;);
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink(&quot;http://www.aspose.com&quot;, &quot;AsposeLink&quot;);

            // Add properties to the smart tag
            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add(&quot;Author&quot;, &quot;Aspose&quot;);
            properties.Add(&quot;Description&quot;, &quot;Aspose.Cells SmartTag&quot;);

            // Save the workbook
            workbook.Save(&quot;SmartTagPropertyDemo.xlsx&quot;);

            Console.WriteLine(&quot;SmartTagPropertyDemo.xlsx created successfully.&quot;);
        }
```

### See Also

* class [SmartTagPropertyCollection](../../smarttagpropertycollection/)
* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


