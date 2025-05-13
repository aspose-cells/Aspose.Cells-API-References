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
public void MarkdownSaveOptions_Property_SheetSet()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
    saveOptions.TableHeaderType = Aspose.Cells.Markdown.MarkdownTableHeaderType.FirstRow;
    saveOptions.SheetSet = SheetSet.All;
    workbook.Save(Constants.destPath + "CELLSJAVA46293.md", saveOptions);
    string text = File.ReadAllText(Constants.destPath + "CELLSJAVA46293.md");
    string text1 = File.ReadAllText(Constants.sourcePath + "CELLSJAVA46293.md");
    Assert.AreEqual(text, text1);
}
```

### See Also

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


