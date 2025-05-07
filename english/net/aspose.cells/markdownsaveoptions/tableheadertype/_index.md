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
// Called: saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
[Test]
        public void Property_TableHeaderType()
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

* enum [MarkdownTableHeaderType](../../../aspose.cells.markdown/markdowntableheadertype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


