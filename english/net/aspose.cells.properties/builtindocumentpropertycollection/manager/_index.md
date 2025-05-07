---
title: BuiltInDocumentPropertyCollection.Manager
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the manager property
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/manager/
---
## BuiltInDocumentPropertyCollection.Manager property

Gets or sets the manager property.

```csharp
public string Manager { get; set; }
```

### Examples

```csharp
// Called: builtInProperties.Manager = "Jane Smith";
public static void Property_Manager()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for test
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            // Access the built-in document properties collection
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Set various built-in document properties
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Sample Workbook";
            builtInProperties.Subject = "Demo";
            builtInProperties.Keywords = "Aspose.Cells, Demo";
            builtInProperties.Comments = "This is a sample workbook created for demonstration purposes.";
            builtInProperties.Company = "Aspose";
            builtInProperties.Category = "Demo Category";
            builtInProperties.ContentType = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet";
            builtInProperties.ContentStatus = "Draft";
            builtInProperties.Language = "en-US";
            builtInProperties.Manager = "Jane Smith";
            builtInProperties.Template = "Standard Template";
            builtInProperties.RevisionNumber = "1";
            builtInProperties.Version = "1.0";
            builtInProperties.DocumentVersion = "1.0";
            builtInProperties.ScaleCrop = true;
            builtInProperties.LinksUpToDate = true;

            // Set date and time properties
            builtInProperties.CreatedTime = DateTime.Now;
            builtInProperties.CreatedUniversalTime = DateTime.UtcNow;
            builtInProperties.LastPrinted = DateTime.Now;
            builtInProperties.LastPrintedUniversalTime = DateTime.UtcNow;
            builtInProperties.LastSavedTime = DateTime.Now;
            builtInProperties.LastSavedUniversalTime = DateTime.UtcNow;

            // Set numeric properties            
            builtInProperties.Pages = 10;
            builtInProperties.Words = 100;
            builtInProperties.TotalEditingTime = 60.0;

            // Save the workbook
            workbook.Save("BuiltInDocumentPropertyCollectionExample.xlsx");
            workbook.Save("BuiltInDocumentPropertyCollectionExample.pdf");

        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


