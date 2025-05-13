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
// Called: b3.InsertText(6, "ttttt");
public void Cell_Method_InsertText()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Cell b3 = workbook.Worksheets[0].Cells["B3"];
    b3.InsertText(6, "ttttt");

    workbook.Save(Constants.destPath + "example.xlsx");

}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


