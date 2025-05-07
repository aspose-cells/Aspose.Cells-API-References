---
title: MarkdownSaveOptions.SheetSet
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Gets or sets the sheets to render. Default is all visible sheets in the workbook Active
type: docs
url: /net/aspose.cells/markdownsaveoptions/sheetset/
---
## MarkdownSaveOptions.SheetSet property

Gets or sets the sheets to render. Default is all visible sheets in the workbook: [`Active`](../../../aspose.cells.rendering/sheetset/active/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Remarks

The set is ignored when it is used in [`SheetRender`](../../../aspose.cells.rendering/sheetrender/)

### Examples

```csharp
// Called: saveOptions.SheetSet = SheetSet.All;
[Test]
        public void Property_SheetSet()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA46318.xlsx");
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            saveOptions.SheetSet = SheetSet.All;
            workbook.Save(Constants.destPath + "CELLSJAVA46318.md", saveOptions);
            string text = File.ReadAllText(Constants.destPath + "CELLSJAVA46318.md");
            Assert.IsTrue(text.IndexOf("---|") != -1);

        }
```

### See Also

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


