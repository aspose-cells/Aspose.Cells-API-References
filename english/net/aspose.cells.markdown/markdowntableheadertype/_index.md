---
title: Enum MarkdownTableHeaderType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Markdown.MarkdownTableHeaderType enum. Represents the header type of the table in the markdown file
type: docs
url: /net/aspose.cells.markdown/markdowntableheadertype/
---
## MarkdownTableHeaderType enumeration

Represents the header type of the table in the markdown file.

```csharp
public enum MarkdownTableHeaderType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| FirstRow | `0` | First row as header of the table. |
| ColumnHeader | `1` | Column name (such as A,B,C...) as header of the table. |
| Empty | `2` | An empty header row. |

### Examples

```csharp
// Called: saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
[Test]
        public void Type_MarkdownTableHeaderType()
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

* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)


