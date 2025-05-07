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
// Called: SaveAsSingleFile=true
[Test]
        public void Property_SaveAsSingleFile()
        {
            Workbook workbook = new Workbook(Constants.HtmlPath + "CELLSJAVA-46349.xlsx");
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html)
            {
                SaveAsSingleFile=true
            }; 
            workbook.Save(_destFilesPath + "CELLSJAVA-46349.html", options);
            workbook = new Workbook(_destFilesPath + "CELLSJAVA-46349.html");
            Assert.AreEqual("DOLLAR INDUSTRIES LIMITED (XNSE:DOLLAR)", workbook.Worksheets[0].Cells["C2"].StringValue);
            Assert.AreEqual("USD/EUR", workbook.Worksheets[0].Cells["C4"].StringValue);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


