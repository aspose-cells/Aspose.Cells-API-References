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
[Test]
        public void Property_TableHeaderType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA46293.xlsx&quot;);
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = Aspose.Cells.Markdown.MarkdownTableHeaderType.FirstRow;
            saveOptions.SheetSet = SheetSet.All;
            workbook.Save(Constants.destPath + &quot;CELLSJAVA46293.md&quot;, saveOptions);
            string text = File.ReadAllText(Constants.destPath + &quot;CELLSJAVA46293.md&quot;);
            string text1 = File.ReadAllText(Constants.sourcePath + &quot;CELLSJAVA46293.md&quot;);
            Assert.AreEqual(text, text1);
        }
```

### See Also

* enum [MarkdownTableHeaderType](../../../aspose.cells.markdown/markdowntableheadertype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


