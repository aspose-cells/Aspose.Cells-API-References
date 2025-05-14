---
title: Cell.Replace
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Replace text of the cell with options
type: docs
url: /net/aspose.cells/cell/replace/
---
## Cell.Replace method

Replace text of the cell with options.

```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |
| options | ReplaceOptions | The replace options |

### Examples

```csharp
// Called: c.Replace(c1.StringValue, c2.StringValue, options1);
public void Cell_Method_Replace()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    Workbook replaceW = new Workbook(Constants.sourcePath + "example.xlsm");
    foreach (Row row in replaceW.Worksheets[0].Cells.Rows)
    {
        Cell c1 = row[0];
        if (string.IsNullOrEmpty(c1.StringValue))
        {
            continue;
        }
        Cell c2 = row[1];
        ReplaceOptions options1 = new ReplaceOptions();
        options1.CaseSensitive = false;
        options1.MatchEntireCellContents = false;
        options1.FontSettings = c2.GetCharacters();
        foreach (Cell c in workbook.Worksheets[0].Cells)
        {
            c.Replace(c1.StringValue, c2.StringValue, options1);
        }
    }
    Cell cell = workbook.Worksheets[0].Cells["D2"];
    FontSetting[] fs = cell.GetCharacters();
    Assert.AreEqual(74, fs[1].StartIndex);
    Assert.AreEqual(FontUnderlineType.None, fs[1].Font.Underline);
    Assert.AreEqual(86, fs[2].StartIndex);
    Assert.AreEqual(FontUnderlineType.Single, fs[2].Font.Underline);
    Util.ReSave(workbook, SaveFormat.Xlsx);
    //workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


