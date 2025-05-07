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
// Called: sorter.AddKey(1, SortOrder.Ascending);
[Test]
        public void Method_SortOrder_() //Cannot reproduce user's issue, no matter using shared formula or normal formulas.
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].SetSharedFormula("=COUNTIF($B$1:$B1,B1)", 1000, 1);
            for (int i = 0; i < 1000; i++)
            {
                cells[i, 1].PutValue(i);
                //cells[i, 0].Formula = "=COUNTIF($B$1:$B" + (i + 1) + ",B" + (i + 1) + ")";
                Assert.AreEqual("=COUNTIF($B$1:$B" + (i + 1) + ",B" + (i + 1) + ")", cells[i, 0].Formula);
            }
            cells[20, 1].PutValue(800);
            cells[800, 1].PutValue(20);
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(1, SortOrder.Ascending);
            sorter.Sort(cells, 0, 0, 999, 1);
            for (int i = 0; i < 1000; i++)
            {
                Assert.AreEqual("=COUNTIF($B$1:$B" + (i + 1) + ",B" + (i + 1) + ")",
                    cells[i, 0].Formula, "A" + (i + 1));
                Assert.AreEqual(i, cells[i, 1].IntValue, "A" + (i + 1));
            }
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
[Test]
        public void Method_String_()
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
            workbook.Save(Constants.destPath + "CELLSNET42150.xlsx");
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


