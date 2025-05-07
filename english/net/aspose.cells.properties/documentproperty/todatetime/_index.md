---
title: DocumentProperty.ToDateTime
second_title: Aspose.Cells for .NET API Reference
description: DocumentProperty method. Returns the property value as DateTime in local timezone
type: docs
url: /net/aspose.cells.properties/documentproperty/todatetime/
---
## DocumentProperty.ToDateTime method

Returns the property value as DateTime in local timezone.

```csharp
public DateTime ToDateTime()
```

### Remarks

Throws an exception if the property type is not PropertyType.Date.

### Examples

```csharp
// Called: Console.WriteLine($"Last Modified: {lastModifiedProperty.ToDateTime()}");
public static void Method_ToDateTime()
        {
            // Instantiate a Workbook object
            Workbook workbook = new Workbook();

            // Retrieve a list of all custom document properties of the Excel file
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Add custom document properties
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Revision", 3);
            customProperties.Add("LastModified", DateTime.Now);
            customProperties.Add("IsFinal", true);
            customProperties.Add("Rating", 4.5);

            // Add a linked custom document property
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");

            // Update linked property values
            //customProperties.UpdateLinkedPropertyValue();
            customProperties.UpdateLinkedRange();

            // Accessing custom document properties
            DocumentProperty authorProperty = customProperties["Author"];
            DocumentProperty revisionProperty = customProperties["Revision"];
            DocumentProperty lastModifiedProperty = customProperties["LastModified"];
            DocumentProperty isFinalProperty = customProperties["IsFinal"];
            DocumentProperty ratingProperty = customProperties["Rating"];
            DocumentProperty linkedProperty = customProperties["LinkedProperty"];

            // Print custom document properties
            Console.WriteLine($"Author: {authorProperty.Value}");
            Console.WriteLine($"Revision: {revisionProperty.ToInt()}");
            Console.WriteLine($"Last Modified: {lastModifiedProperty.ToDateTime()}");
            Console.WriteLine($"Is Final: {isFinalProperty.ToBool()}");
            Console.WriteLine($"Rating: {ratingProperty.ToDouble()}");
            Console.WriteLine($"Linked Property: {linkedProperty.Value}");

            // Save the workbook
            workbook.Save("CustomDocumentPropertiesExample.xlsx");
            workbook.Save("CustomDocumentPropertiesExample.pdf");
        }
```

### See Also

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


