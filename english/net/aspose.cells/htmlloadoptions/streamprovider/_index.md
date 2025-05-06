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
public static void Property_StreamProvider()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set some data in the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello World&quot;);

            // Create HtmlSaveOptions and set the StreamProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new IStreamProviderDemo();

            // Save the workbook to HTML format
            workbook.Save(&quot;IStreamProviderExample.html&quot;, saveOptions);

            // Load the workbook from HTML format
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new IStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook(&quot;IStreamProviderExample.html&quot;, loadOptions);

            // Display the loaded data
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells[&quot;A1&quot;].StringValue);
        }
```

### See Also

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


