---
title: SheetSet.All
second_title: Aspose.Cells for .NET API Reference
description: SheetSet property. Gets a set with all sheets of the workbook in their original order
type: docs
url: /net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

Gets a set with all sheets of the workbook in their original order.

```csharp
public static SheetSet All { get; }
```

### Examples

```csharp
// Called: saveOptions.SheetSet = SheetSet.All;
public void SheetSet_Property_All()
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

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


