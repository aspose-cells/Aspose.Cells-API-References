---
title: BuiltInDocumentPropertyCollection.Company
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the company property
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/company/
---
## BuiltInDocumentPropertyCollection.Company property

Gets or sets the company property.

```csharp
public string Company { get; set; }
```

### Examples

```csharp
// Called: builtInProperties.Company = &amp;quot;Aspose&amp;quot;;
public static void Property_Company()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the built-in document properties
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Set some built-in properties
            builtInProperties.Author = &quot;John Doe&quot;;
            builtInProperties.Title = &quot;Sample Workbook&quot;;
            builtInProperties.Subject = &quot;Demonstration of PropertyType&quot;;
            builtInProperties.Company = &quot;Aspose&quot;;

            // Access the custom document properties
            CustomDocumentPropertyCollection customProperties = workbook.CustomDocumentProperties;

            // Add custom properties of different types
            customProperties.Add(&quot;IsReviewed&quot;, true); // Boolean
            customProperties.Add(&quot;ReviewDate&quot;, DateTime.Now); // DateTime
            customProperties.Add(&quot;Rating&quot;, 4.5); // Double
            customProperties.Add(&quot;Pages&quot;, 100); // Number
            customProperties.Add(&quot;Summary&quot;, &quot;This is a sample workbook for demonstrating PropertyType.&quot;); // String

            // Retrieve and display custom properties
            foreach (DocumentProperty property in customProperties)
            {
                Console.WriteLine($&quot;Name: {property.Name}, Value: {property.Value}, Type: {property.Type}&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;PropertyTypeExample.xlsx&quot;);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


