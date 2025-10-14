---
title: CustomDocumentPropertyCollection.UpdateLinkedPropertyValue
second_title: Aspose.Cells for .NET API Reference
description: CustomDocumentPropertyCollection method. Updates values of all custom properties that are linked to contentuse cell value of linked range to update value of custom property
type: docs
url: /net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/
---
## CustomDocumentPropertyCollection.UpdateLinkedPropertyValue method

Updates values of all custom properties that are linked to content(use cell value of linked range to update value of custom property).

```csharp
public void UpdateLinkedPropertyValue()
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedPropertyValueDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Add some data to cells that will be linked to custom properties
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "InitialValue1";
            worksheet.Cells["B1"].Value = "InitialValue2";

            // Add linked custom properties
            workbook.CustomDocumentProperties.AddLinkToContent("CompanyName", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Department", "B1");

            // Update the cell values
            worksheet.Cells["A1"].Value = "UpdatedValue1";
            worksheet.Cells["B1"].Value = "UpdatedValue2";

            // Update the linked property values
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Display the updated property values
            Console.WriteLine("CompanyName: " + workbook.CustomDocumentProperties["CompanyName"].Value);
            Console.WriteLine("Department: " + workbook.CustomDocumentProperties["Department"].Value);

            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


