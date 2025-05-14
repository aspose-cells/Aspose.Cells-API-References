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
public static void PaginatedSaveOptions_Property_PageSavingCallback()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Create save options with a page saving callback
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.PageSavingCallback = new PageSavingCallbackDemo();

            // Save the workbook as a DOCX file
            workbook.Save("PageSavingCallbackExample.docx", saveOptions);
        }
```

### See Also

* interface [IPageSavingCallback](../../../aspose.cells.rendering/ipagesavingcallback/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


