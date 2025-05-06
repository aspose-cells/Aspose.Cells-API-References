---
title: Cell.InsertText
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Insert some characters to the cell. If the cell is rich formatted this method could keep the original formatting
type: docs
url: /net/aspose.cells/cell/inserttext/
---
## Cell.InsertText method

Insert some characters to the cell. If the cell is rich formatted, this method could keep the original formatting.

```csharp
public void InsertText(int index, string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index. |
| text | String | Inserted text. |

### Examples

```csharp
// Called: b3.InsertText(6, &amp;quot;ttttt&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET53887.xlsx&quot;);
            Cell b3 = workbook.Worksheets[0].Cells[&quot;B3&quot;];
            b3.InsertText(6, &quot;ttttt&quot;);

            workbook.Save(Constants.destPath + &quot;CELLSNET53887.xlsx&quot;);

        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


