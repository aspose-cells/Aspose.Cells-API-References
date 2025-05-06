---
title: BuiltInDocumentPropertyCollection.LastSavedUniversalTime
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the universal time of the last save
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/lastsaveduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastSavedUniversalTime property

Gets or sets the universal time of the last save.

```csharp
public DateTime LastSavedUniversalTime { get; set; }
```

### Remarks

Aspose.Cells does not update this property when you modify the document.

### Examples

```csharp
// Called: builtInProperties.LastSavedUniversalTime = DateTime.UtcNow;
public static void Property_LastSavedUniversalTime()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for test
            worksheet.Cells[&quot;A1&quot;].PutValue(1);
            worksheet.Cells[&quot;A2&quot;].PutValue(2);
            worksheet.Cells[&quot;A3&quot;].PutValue(3);
            worksheet.Cells[&quot;B1&quot;].PutValue(2);
            worksheet.Cells[&quot;B2&quot;].PutValue(3);
            worksheet.Cells[&quot;B3&quot;].PutValue(4);
            worksheet.Cells[&quot;C1&quot;].PutValue(5);
            worksheet.Cells[&quot;C2&quot;].PutValue(10);
            worksheet.Cells[&quot;C3&quot;].PutValue(15);

            // Access the built-in document properties collection
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Set various built-in document properties
            builtInProperties.Author = &quot;John Doe&quot;;
            builtInProperties.Title = &quot;Sample Workbook&quot;;
            builtInProperties.Subject = &quot;Demo&quot;;
            builtInProperties.Keywords = &quot;Aspose.Cells, Demo&quot;;
            builtInProperties.Comments = &quot;This is a sample workbook created for demonstration purposes.&quot;;
            builtInProperties.Company = &quot;Aspose&quot;;
            builtInProperties.Category = &quot;Demo Category&quot;;
            builtInProperties.ContentType = &quot;application/vnd.openxmlformats-officedocument.spreadsheetml.sheet&quot;;
            builtInProperties.ContentStatus = &quot;Draft&quot;;
            builtInProperties.Language = &quot;en-US&quot;;
            builtInProperties.Manager = &quot;Jane Smith&quot;;
            builtInProperties.Template = &quot;Standard Template&quot;;
            builtInProperties.RevisionNumber = &quot;1&quot;;
            builtInProperties.Version = &quot;1.0&quot;;
            builtInProperties.DocumentVersion = &quot;1.0&quot;;
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
            workbook.Save(&quot;BuiltInDocumentPropertyCollectionExample.xlsx&quot;);
            workbook.Save(&quot;BuiltInDocumentPropertyCollectionExample.pdf&quot;);

        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


