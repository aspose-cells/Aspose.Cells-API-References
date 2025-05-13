---
title: DataSorter.AddKey
second_title: Aspose.Cells for .NET API Reference
description: DataSorter method. Adds sorted column index and sort order
type: docs
url: /net/aspose.cells/datasorter/addkey/
---
## AddKey(int, SortOrder) {#addkey_1}

Adds sorted column index and sort order.

```csharp
public void AddKey(int key, SortOrder order)
```

| Parameter | Type | Description |
| --- | --- | --- |
| key | Int32 | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | SortOrder | The sort order |

### Examples

```csharp
// Called: workbook.DataSorter.AddKey(5, SortOrder.Ascending);
// Does Aspose.Cells have ability to add sort fields to ListObjects
// http://www.aspose.com/community/forums/thread/292632.aspx
public void DataSorter_Method_AddKey()
{
    Console.WriteLine("DataSorter_Method_AddKey()");
    string infn = path + @"ListObjectSort\ListObjectSort.xlsx";
    string outfn = Constants.destPath + @"ListObjectSort_out.xlsx";

    Workbook workbook = new Workbook(infn);
    workbook.DataSorter.AddKey(5, SortOrder.Ascending);
    workbook.DataSorter.Sort(workbook.Worksheets[0].Cells, 4, 3, 6, 5);
    Assert.LessOrEqual(workbook.Worksheets[0].Cells["F5"].IntValue,
        workbook.Worksheets[0].Cells["F6"].IntValue);
    Assert.LessOrEqual(workbook.Worksheets[0].Cells["F6"].IntValue,
        workbook.Worksheets[0].Cells["F7"].IntValue);
    workbook.Save(outfn, SaveFormat.Xlsx);
}
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string) {#addkey_2}

Adds sorted column index and sort order with custom sort list.

```csharp
public void AddKey(int key, SortOrder order, string customList)
```

| Parameter | Type | Description |
| --- | --- | --- |
| key | Int32 | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | SortOrder | The sort order. |
| customList | String | The custom sort list. |

### Examples

```csharp
// Called: sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
public void DataSorter_Method_AddKey()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Sort/File_for_CustomSort_ASPOSE_Forum_Question.xlsx");
    DataSorter sorter = workbook.DataSorter;
    sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
    sorter.HasHeaders = true;
    sorter.Sort(workbook.Worksheets[1].Cells, CellArea.CreateCellArea("A1", "C23"));
    Cells cells = workbook.Worksheets[1].Cells;
    Assert.AreEqual(cells["A2"].StringValue, "aaa");
    Assert.AreEqual(cells["A7"].StringValue, "ddd");
    Assert.AreEqual(cells["A12"].StringValue, "ccc");
    Assert.AreEqual(cells["A18"].StringValue, "bbb");
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOnType, SortOrder, object) {#addkey}

Adds sorted column index and sort order with custom sort list.

```csharp
public void AddKey(int key, SortOnType type, SortOrder order, object customList)
```

| Parameter | Type | Description |
| --- | --- | --- |
| key | Int32 | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | SortOnType | The sorted value type. |
| order | SortOrder | The sort order. |
| customList | Object | The custom sort list. |

### Remarks

If type is SortOnType.CellColor or SortOnType.FontColor, the customList is Color.

### See Also

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string[]) {#addkey_3}

Adds sorted column index and sort order with custom sort list.

```csharp
public void AddKey(int key, SortOrder order, string[] customList)
```

| Parameter | Type | Description |
| --- | --- | --- |
| key | Int32 | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | SortOrder | The sort order. |
| customList | String[] | The custom sort list. |

### See Also

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


