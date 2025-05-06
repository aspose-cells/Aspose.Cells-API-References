---
title: DataSorter.AddColorKey
second_title: Aspose.Cells for .NET API Reference
description: DataSorter method. Adds color sort key
type: docs
url: /net/aspose.cells/datasorter/addcolorkey/
---
## DataSorter.AddColorKey method

Adds color sort key.

```csharp
public void AddColorKey(int key, SortOnType type, SortOrder order, Color color)
```

| Parameter | Type | Description |
| --- | --- | --- |
| key | Int32 | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | SortOnType | The sorted color value type. |
| order | SortOrder | The sort order. |
| color | Color | The custom sort color. |

### Examples

```csharp
// Called: sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);
[Test]
        public void Method_Color_()
        {
            //CELLSNET-57170
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSCPP1130.xlsx&quot;);
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.AddColorKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Red);
            sorter.Sort(workbook.Worksheets[0].Cells, CellArea.CreateCellArea(0, 0, 4, 3));
            Assert.AreEqual(5, workbook.Worksheets[0].Cells[&quot;A2&quot;].IntValue);
        }
```

### See Also

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


