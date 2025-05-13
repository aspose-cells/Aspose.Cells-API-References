---
title: HtmlLoadOptions.StreamProvider
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Gets or sets the StreamProviderImportHtmlFile for importing objects
type: docs
url: /net/aspose.cells/htmlloadoptions/streamprovider/
---
## HtmlLoadOptions.StreamProvider property

Gets or sets the StreamProviderImportHtmlFile for importing objects.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Examples

```csharp
// Called: loadOptions.StreamProvider = new IStreamProviderDemo();
public static void HtmlLoadOptions_Property_StreamProvider()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set some data in the worksheet
            worksheet.Cells["A1"].PutValue("Hello World");

            // Create HtmlSaveOptions and set the StreamProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new IStreamProviderDemo();

            // Save the workbook to HTML format
            workbook.Save("IStreamProviderExample.html", saveOptions);

            // Load the workbook from HTML format
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new IStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("IStreamProviderExample.html", loadOptions);

            // Display the loaded data
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
```

### See Also

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


