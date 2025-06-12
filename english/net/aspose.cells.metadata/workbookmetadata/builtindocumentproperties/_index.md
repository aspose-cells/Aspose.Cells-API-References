---
title: WorkbookMetadata.BuiltInDocumentProperties
second_title: Aspose.Cells for .NET API Reference
description: WorkbookMetadata property. Returns a DocumentProperty collection that represents all the builtin document properties of the spreadsheet
type: docs
url: /net/aspose.cells.metadata/workbookmetadata/builtindocumentproperties/
---
## WorkbookMetadata.BuiltInDocumentProperties property

Returns a [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) collection that represents all the built-in document properties of the spreadsheet.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access built-in document properties
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
            
            // Set some built-in properties using the proper methods
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Author = "John Doe";
            builtInProperties.Company = "Aspose";
            builtInProperties.Comments = "This demonstrates BuiltInDocumentProperties usage";
            
            // Display the properties
            Console.WriteLine("Title: " + builtInProperties.Title);
            Console.WriteLine("Author: " + builtInProperties.Author);
            Console.WriteLine("Company: " + builtInProperties.Company);
            Console.WriteLine("Comments: " + builtInProperties.Comments);
            
            // Save the workbook
            workbook.Save("BuiltInDocumentPropertiesDemo.xlsx");
            
            Console.WriteLine("Workbook with built-in properties saved successfully.");
        }
    }
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


