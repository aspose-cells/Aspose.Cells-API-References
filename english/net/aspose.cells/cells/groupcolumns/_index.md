---
title: Cells.GroupColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Groups columns
type: docs
url: /net/aspose.cells/cells/groupcolumns/
---
## GroupColumns(int, int) {#groupcolumns}

Groups columns.

```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first column index to be grouped. |
| lastIndex | Int32 | The last column index to be grouped. |

### Examples

```csharp
// Called: cells.GroupColumns(0, 2);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.GroupColumns(0, 2);
            Aspose.Cells.Range range = cells.CreateRange(0, 3, true);
            Aspose.Cells.Range range2 = cells.CreateRange(5, 3, true);
            range2.Copy(range);
            Assert.AreEqual(cells.Columns[5].GroupLevel, 1);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupColumns(int, int, bool) {#groupcolumns_1}

Groups columns.

```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first column index to be grouped. |
| lastIndex | Int32 | The last column index to be grouped. |
| isHidden | Boolean | Specifies if the grouped columns are hidden. |

### Examples

```csharp
// Called: cells.GroupColumns(4, 4, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Outline.SummaryRowBelow = false;
            sheet.Outline.SummaryColumnRight = false;
            Cells cells = wb.Worksheets[0].Cells;
            string[] ovs = new string[] {
                &quot;A&quot;, &quot;AA&quot;, &quot;A&quot;, &quot;AD&quot;, &quot;A&quot;, &quot;AC&quot;, &quot;C&quot;, &quot;CB&quot;, &quot;C&quot;, &quot;CA&quot;, &quot;B&quot;, &quot;BD&quot;, &quot;B&quot;, &quot;BC&quot;, &quot;B&quot;, &quot;BF&quot;
            };
            for (int i = 0; i &lt; ovs.Length; i++)
            {
                cells[i / 2, i % 2].PutValue(ovs[i]);
            }

            cells.GroupRows(1, 2, true);
            cells.GroupRows(4, 4, true);
            cells.GroupRows(6, 7, true);
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            sorter.AddKey(1, SortOrder.Ascending);

            sorter.Sort(cells, 0, 0, 7, 1);
            string[] nvs = new string[] { &quot;A&quot;,&quot;AA&quot;,&quot;A&quot;,&quot;AD&quot;,&quot;A&quot;,&quot;AC&quot;,&quot;B&quot;,&quot;BD&quot;,&quot;B&quot;,&quot;BC&quot;,&quot;B&quot;,&quot;BF&quot;,&quot;C&quot;,&quot;CB&quot;,&quot;C&quot;,&quot;CA&quot; };
            int[] groups = new int[] { 0, 1, 1, 0, 1, 1, 0, 1 };
            for (int i = 0; i &lt; nvs.Length; i++)
            {
                Assert.AreEqual(nvs[i], cells[i / 2, i % 2].Value, &quot;Item-Row-&quot; + i);
            }
            for (int i = 0; i &lt; groups.Length; i++)
            {
                Assert.AreEqual(groups[i] &gt; 0, cells.Rows[i].IsHidden, &quot;Hidden-Row-&quot; + i);
                Assert.AreEqual(groups[i], cells.Rows[i].GroupLevel, &quot;GroupLevel-Row-&quot; + i);
            }

            cells.Clear();
            for (int i = 0; i &lt; ovs.Length; i++)
            {
                cells[i % 2, i / 2].PutValue(ovs[i]);
            }

            cells.GroupColumns(1, 2, true);
            cells.GroupColumns(4, 4, true);
            cells.GroupColumns(6, 7, true);
            sorter.SortLeftToRight = true;
            sorter.Sort(cells, 0, 0, 1, 7);
            for (int i = 0; i &lt; nvs.Length; i++)
            {
                Assert.AreEqual(nvs[i], cells[i % 2, i / 2].Value, &quot;Item-Column-&quot; + i);
            }
            for (int i = 10; i &lt; groups.Length; i++) //currently we do not support to exchange the group settings for column
            {
                Assert.AreEqual(groups[i] &gt; 0, cells.Columns[i].IsHidden, &quot;Hidden-Column-&quot; + i);
                Assert.AreEqual(groups[i], cells.Columns[i].GroupLevel, &quot;GroupLevel-Column-&quot; + i);
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


