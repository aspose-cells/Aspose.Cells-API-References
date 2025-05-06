---
title: PaginatedSaveOptions.PageSavingCallback
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Control/Indicate progress of page saving process
type: docs
url: /net/aspose.cells/paginatedsaveoptions/pagesavingcallback/
---
## PaginatedSaveOptions.PageSavingCallback property

Control/Indicate progress of page saving process.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### Examples

```csharp
// Called: saveOptions.PageSavingCallback = new PageSavingCallbackDemo();
public static void Property_PageSavingCallback()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;World&quot;);

            // Create save options with a page saving callback
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.PageSavingCallback = new PageSavingCallbackDemo();

            // Save the workbook as a DOCX file
            workbook.Save(&quot;PageSavingCallbackExample.docx&quot;, saveOptions);
        }
```

### See Also

* interface [IPageSavingCallback](../../../aspose.cells.rendering/ipagesavingcallback/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


