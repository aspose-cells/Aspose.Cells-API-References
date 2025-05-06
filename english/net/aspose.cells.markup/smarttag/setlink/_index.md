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
// Called: smartTag.SetLink(&amp;quot;http://www.aspose.com&amp;quot;, &amp;quot;AsposeLink&amp;quot;);
public static void Method_String_()
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

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


