---
title: Cell.StringValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the string value contained in the cell. If the type of this cell is string then return the string value itself. For other cell types the formatted string value formatted with the specified style of this cell will be returned. The formatted cell value is same with what you can get from excel when copying a cell as textsuch as copying cell to text editor or exporting to csv
type: docs
url: /net/aspose.cells/cell/stringvalue/
---
## Cell.StringValue property

Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself. For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned. The formatted cell value is same with what you can get from excel when copying a cell as text(such as copying cell to text editor or exporting to csv).

```csharp
public string StringValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells[&amp;quot;C2&amp;quot;].StringValue, &amp;quot;粮油组&amp;quot;);
[Test]
        public void Property_StringValue()
        {
            //Only GB2312 encoding can decode the file correctly.
            if (Encoding.Default.CodePage == 936)
            {
                Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET50323.xls&quot;);
                Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;C2&quot;].StringValue, &quot;粮油组&quot;);
                workbook.Save(Constants.destPath + &quot;CELLSNET50323.xlsx&quot;);
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


