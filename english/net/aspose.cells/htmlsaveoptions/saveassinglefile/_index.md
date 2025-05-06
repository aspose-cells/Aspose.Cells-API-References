---
title: HtmlSaveOptions.SaveAsSingleFile
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether save the html as single file. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/saveassinglefile/
---
## HtmlSaveOptions.SaveAsSingleFile property

Indicates whether save the html as single file. The default value is false.

```csharp
public bool SaveAsSingleFile { get; set; }
```

### Remarks

If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.

### Examples

```csharp
// Called: SaveAsSingleFile = true
[Test]
        public void Property_SaveAsSingleFile()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSAPP1434.xlsx&quot;);

            HtmlSaveOptions SaveOptions = new HtmlSaveOptions(SaveFormat.MHtml)
            {
                ExportImagesAsBase64 = true,
                SaveAsSingleFile = true
            };

            workbook.Save(Constants.destPath + &quot;CELLSAPP1434.mht&quot;, SaveOptions);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


