---
title: Worksheet.CustomProperties
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets an object representing the identifier information associated with a worksheet
type: docs
url: /net/aspose.cells/worksheet/customproperties/
---
## Worksheet.CustomProperties property

Gets an object representing the identifier information associated with a worksheet.

```csharp
public CustomPropertyCollection CustomProperties { get; }
```

### Remarks

Worksheet.CustomProperties provide a preferred mechanism for storing arbitrary data. It supports legacy third-party document components, as well as those situations that have a stringent need for binary parts.

### Examples

```csharp
// Called: CustomPropertyCollection customProperties = worksheet.CustomProperties;
public static void Property_CustomProperties()
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

* class [CustomPropertyCollection](../../../aspose.cells.properties/custompropertycollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


