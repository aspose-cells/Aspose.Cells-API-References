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
// Called: sorter.AddKey(0, SortOrder.Descending);
[Test]
        public void Method_SortOrder_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            Random rdm = new Random();
            for (int i = 0; i &lt; 200; i++)
            {
                int index = (int)(rdm.NextDouble() * 100);
                string columnName = CellsHelper.ColumnIndexToName(index);
                for (int j = 1; j &lt; 10; j++)
                {
                    cells[&quot;A&quot; + (i * 10 + j)].PutValue(columnName + &quot;A&quot; + i);
                    cells[&quot;B&quot; + (i * 10 + j)].PutValue(columnName + &quot;B&quot; +(index * 10 + j));
                    cells[&quot;C&quot; + (i * 10 + j)].PutValue(columnName + &quot;C&quot; + j);
                    cells[&quot;D&quot; + (i * 10 + j)].PutValue(columnName + &quot;D&quot; +(i * 10 + j));
                }
                cells.GroupRows((i * 10 + 1), (i * 10 + 9), true);
            }
            sheet.Outline.SummaryRowBelow = false;
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(2, SortOrder.Ascending);
            sorter.AddKey(0, SortOrder.Descending);
            sorter.AddKey(1, SortOrder.Descending);
            sorter.Sort(cells, 0, 0, 2000, 4); //here should not give exception
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
// Called: sorter.AddKey(0, SortOrder.Ascending, &amp;quot;aaa,ddd,ccc,bbb&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Sort/File_for_CustomSort_ASPOSE_Forum_Question.xlsx&quot;);
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, &quot;aaa,ddd,ccc,bbb&quot;);
            sorter.HasHeaders = true;
            sorter.Sort(workbook.Worksheets[1].Cells, CellArea.CreateCellArea(&quot;A1&quot;, &quot;C23&quot;));
            Cells cells = workbook.Worksheets[1].Cells;
            Assert.AreEqual(cells[&quot;A2&quot;].StringValue, &quot;aaa&quot;);
            Assert.AreEqual(cells[&quot;A7&quot;].StringValue, &quot;ddd&quot;);
            Assert.AreEqual(cells[&quot;A12&quot;].StringValue, &quot;ccc&quot;);
            Assert.AreEqual(cells[&quot;A18&quot;].StringValue, &quot;bbb&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSNET42150.xlsx&quot;);
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


