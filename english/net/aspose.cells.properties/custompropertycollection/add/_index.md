---
title: CustomPropertyCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: CustomPropertyCollection method. Adds custom property information
type: docs
url: /net/aspose.cells.properties/custompropertycollection/add/
---
## CustomPropertyCollection.Add method

Adds custom property information.

```csharp
public int Add(string name, string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the custom property. |
| value | String | The value of the custom property. |

### Examples

```csharp
// Called: customProperties.Add(&amp;quot;Version&amp;quot;, &amp;quot;1.0&amp;quot;);
public static void Method_String_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Access the CustomProperties collection
            CustomPropertyCollection customProperties = sheet.CustomProperties;

            // Add custom properties
            customProperties.Add(&quot;Author&quot;, &quot;John Doe&quot;);
            customProperties.Add(&quot;Version&quot;, &quot;1.0&quot;);
            customProperties.Add(&quot;LastModified&quot;, DateTime.Now.ToString());

            // Access and display custom properties
            for (int i = 0; i &lt; customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($&quot;Name: {property.Name}, Value: {property.Value}&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;CustomPropertyExample.xlsx&quot;);
            workbook.Save(&quot;CustomPropertyExample.pdf&quot;);
        }
```

### See Also

* class [CustomPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


