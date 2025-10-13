---
title: CustomDocumentPropertyCollection.UpdateLinkedRange
second_title: Aspose.Cells for .NET API Reference
description: CustomDocumentPropertyCollection method. Updates all ranges that are linked to custom propertiesuse the value of custom document property to update cell value of linked range
type: docs
url: /net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/
---
## CustomDocumentPropertyCollection.UpdateLinkedRange method

Updates all ranges that are linked to custom properties(use the value of custom document property to update cell value of linked range).

```csharp
public void UpdateLinkedRange()
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Set a value in cell A1 that will be linked
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Add a linked property
            customProperties.AddLinkToContent("LinkedRange", "Sheet1!A1");
            
            // Update all linked properties
            customProperties.UpdateLinkedRange();
            
            // Get and display the linked property value
            DocumentProperty linkedProp = customProperties["LinkedRange"];
            Console.WriteLine($"Linked Property Value: {linkedProp.Value}");

            // Save the workbook
            workbook.Save("LinkedRangeExample.xlsx");
        }
    }
}
```

### See Also

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


