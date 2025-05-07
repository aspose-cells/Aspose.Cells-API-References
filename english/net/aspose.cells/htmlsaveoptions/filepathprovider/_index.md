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
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Create HtmlSaveOptions and set the FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // Save the workbook to HTML format
            workbook.Save("IFilePathProviderExample.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
```

### See Also

* interface [IFilePathProvider](../../ifilepathprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


