---
title: HtmlSaveOptions.CellCssPrefix
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets and sets the prefix of the css namethe default value is 
type: docs
url: /net/aspose.cells/htmlsaveoptions/cellcssprefix/
---
## HtmlSaveOptions.CellCssPrefix property

Gets and sets the prefix of the css name,the default value is "".

```csharp
public string CellCssPrefix { get; set; }
```

### Examples

```csharp
// Called: CellCssPrefix = "cssPrefix"
[Test]
        public void Property_CellCssPrefix()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45306/";

            var workbook = new Workbook(filePath + @"test.xlsx");
            workbook.Worksheets[0].Cells["M4"].Characters(0, 10).Font.Color = Color.Red;
            workbook.Save(CreateFolder(filePath) + @"out.html", new HtmlSaveOptions(SaveFormat.Html)
            {
                CellCssPrefix = "cssPrefix"
            });


        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


