---
title: CustomProperty.Name
second_title: Aspose.Cells for .NET API Reference
description: CustomProperty property. Returns or sets the name of the object
type: docs
url: /net/aspose.cells.properties/customproperty/name/
---
## CustomProperty.Name property

Returns or sets the name of the object.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine($&amp;quot;Name: {property.Name}, Value: {property.Value}&amp;quot;);
public static void Property_Name()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the CustomPropertyCollection of the worksheet
            CustomPropertyCollection customProperties = worksheet.CustomProperties;

            // Add custom properties
            customProperties.Add(&quot;Author&quot;, &quot;John Doe&quot;);
            customProperties.Add(&quot;Version&quot;, &quot;1.0&quot;);

            // Access and print the custom properties
            for (int i = 0; i &lt; customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($&quot;Name: {property.Name}, Value: {property.Value}&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;CustomPropertyCollectionExample.xlsx&quot;);
            workbook.Save(&quot;CustomPropertyCollectionExample.pdf&quot;);
            return;
        }
```

### See Also

* class [CustomProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


