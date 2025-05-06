---
title: HtmlSaveOptions.FilePathProvider
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets or sets the IFilePathProvider for exporting Worksheet to html separately
type: docs
url: /net/aspose.cells/htmlsaveoptions/filepathprovider/
---
## HtmlSaveOptions.FilePathProvider property

Gets or sets the IFilePathProvider for exporting Worksheet to html separately.

```csharp
public IFilePathProvider FilePathProvider { get; set; }
```

### Examples

```csharp
// Called: saveOptions.FilePathProvider = new IFilePathProviderDemo();
public static void Property_FilePathProvider()
        {
            // Create a new workbook and add some data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;World&quot;);

            // Create HtmlSaveOptions and set the FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // Save the workbook to HTML format
            workbook.Save(&quot;IFilePathProviderExample.html&quot;, saveOptions);

            Console.WriteLine(&quot;Workbook saved to HTML with custom file paths.&quot;);
        }
```

### See Also

* interface [IFilePathProvider](../../ifilepathprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


