---
title: WorksheetCollection.CreateUnionRange
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Creates a Range object from an address of the range
type: docs
url: /net/aspose.cells/worksheetcollection/createunionrange/
---
## WorksheetCollection.CreateUnionRange method

Creates a [`Range`](../../range/) object from an address of the range.

```csharp
public UnionRange CreateUnionRange(string address, int sheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |
| sheetIndex | Int32 | The sheet index. |

### Return Value

A [`Range`](../../range/) object

### Examples

```csharp
// Called: UnionRange r = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
public void WorksheetCollection_Method_CreateUnionRange()
{
    Workbook workbook = new Workbook();
    UnionRange r = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
    Assert.IsTrue(r.HasRange);
    r.Value = "ABCD";
    Style style = workbook.CreateStyle();
    style.Pattern = BackgroundType.Solid;
    style.ForegroundColor = System.Drawing.Color.Red;
    workbook.Save(Constants.destPath + "example.xlsx");

}
```

### See Also

* class [UnionRange](../../unionrange/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


