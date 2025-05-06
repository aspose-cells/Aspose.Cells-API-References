---
title: HtmlSaveOptions.StreamProvider
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets or sets the IStreamProvider for exporting objects
type: docs
url: /net/aspose.cells/htmlsaveoptions/streamprovider/
---
## HtmlSaveOptions.StreamProvider property

Gets or sets the IStreamProvider for exporting objects.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Examples

```csharp
// Called: options.StreamProvider = new ExportStreamProvider(CreateFolder(outputDir));
[Test]
        public void Property_StreamProvider()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET43250/&quot;;
            string outputDir = filePath + @&quot;out/&quot;;
            Workbook wb = new Workbook(filePath + &quot;a.xlsx&quot;);
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.StreamProvider = new ExportStreamProvider(CreateFolder(outputDir));
            wb.Save(CreateFolder(filePath) + &quot;out.html&quot;, options);
        }
```

### See Also

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


