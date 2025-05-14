---
title: MarkdownSaveOptions.TableHeaderType
second_title: Aspose.Cells for .NET API Reference
description: MarkdownSaveOptions property. Gets and sets how set the header of the table
type: docs
url: /net/aspose.cells/markdownsaveoptions/tableheadertype/
---
## MarkdownSaveOptions.TableHeaderType property

Gets and sets how set the header of the table.

```csharp
public MarkdownTableHeaderType TableHeaderType { get; set; }
```

### Examples

```csharp
// Called: saveOptions.TableHeaderType = Aspose.Cells.Markdown.MarkdownTableHeaderType.FirstRow;
public void MarkdownSaveOptions_Property_TableHeaderType()
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

* enum [MarkdownTableHeaderType](../../../aspose.cells.markdown/markdowntableheadertype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


