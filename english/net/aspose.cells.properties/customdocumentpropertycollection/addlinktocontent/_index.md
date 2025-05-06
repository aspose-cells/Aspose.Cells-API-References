---
title: CustomDocumentPropertyCollection.AddLinkToContent
second_title: Aspose.Cells for .NET API Reference
description: CustomDocumentPropertyCollection method. Creates a new custom document property which links to content
type: docs
url: /net/aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/
---
## CustomDocumentPropertyCollection.AddLinkToContent method

Creates a new custom document property which links to content.

```csharp
public DocumentProperty AddLinkToContent(string name, string source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the property. |
| source | String | The source of the property. It should be the name of named range. |

### Return Value

The newly created property object.

### Examples

```csharp
// Called: customProperties.AddLinkToContent(&amp;quot;LinkedProperty&amp;quot;, &amp;quot;Sheet1!A1&amp;quot;);
public static void Method_String_()
        {
            // Instantiate a Workbook object
            Workbook workbook = new Workbook();

            // Retrieve a list of all custom document properties of the Excel file
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Add custom document properties
            customProperties.Add(&quot;Author&quot;, &quot;John Doe&quot;);
            customProperties.Add(&quot;Revision&quot;, 3);
            customProperties.Add(&quot;LastModified&quot;, DateTime.Now);
            customProperties.Add(&quot;IsFinal&quot;, true);
            customProperties.Add(&quot;Rating&quot;, 4.5);

            // Add a linked custom document property
            customProperties.AddLinkToContent(&quot;LinkedProperty&quot;, &quot;Sheet1!A1&quot;);

            // Update linked property values
            //customProperties.UpdateLinkedPropertyValue();
            customProperties.UpdateLinkedRange();

            // Accessing custom document properties
            DocumentProperty authorProperty = customProperties[&quot;Author&quot;];
            DocumentProperty revisionProperty = customProperties[&quot;Revision&quot;];
            DocumentProperty lastModifiedProperty = customProperties[&quot;LastModified&quot;];
            DocumentProperty isFinalProperty = customProperties[&quot;IsFinal&quot;];
            DocumentProperty ratingProperty = customProperties[&quot;Rating&quot;];
            DocumentProperty linkedProperty = customProperties[&quot;LinkedProperty&quot;];

            // Print custom document properties
            Console.WriteLine($&quot;Author: {authorProperty.Value}&quot;);
            Console.WriteLine($&quot;Revision: {revisionProperty.ToInt()}&quot;);
            Console.WriteLine($&quot;Last Modified: {lastModifiedProperty.ToDateTime()}&quot;);
            Console.WriteLine($&quot;Is Final: {isFinalProperty.ToBool()}&quot;);
            Console.WriteLine($&quot;Rating: {ratingProperty.ToDouble()}&quot;);
            Console.WriteLine($&quot;Linked Property: {linkedProperty.Value}&quot;);

            // Save the workbook
            workbook.Save(&quot;CustomDocumentPropertiesExample.xlsx&quot;);
            workbook.Save(&quot;CustomDocumentPropertiesExample.pdf&quot;);
        }
```

### See Also

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


