---
title: Cells.GroupRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Groups rows
type: docs
url: /net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

Groups rows.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be grouped. |
| lastIndex | Int32 | The last row index to be grouped. |
| isHidden | Boolean | Specifies if the grouped rows are hidden. |

### Examples

```csharp
// Called: worksheet1.Cells.GroupRows(2, 4, false);
[Test]
        public void Method_Boolean_()
        {

            var workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            var worksheet1 = workbook.Worksheets[0];
            var worksheet2 = workbook.Worksheets[1];
            var worksheet3 = workbook.Worksheets[2];
            var worksheet4 = workbook.Worksheets[3];
            worksheet1.Outline.SummaryRowBelow = false;
            worksheet2.Outline.SummaryRowBelow = false;
            worksheet3.Outline.SummaryRowBelow = false;
            worksheet4.Outline.SummaryRowBelow = false;

            //for (int i = 1; i &lt;= 9; ++i)
            //{
            //    worksheet1.Cells[$&quot;A{i}&quot;].PutValue($&quot;Row{i}&quot;);
            //    worksheet2.Cells[$&quot;A{i}&quot;].PutValue($&quot;Row{i}&quot;);
            //    worksheet3.Cells[$&quot;A{i}&quot;].PutValue($&quot;Row{i}&quot;);
            //    worksheet4.Cells[$&quot;A{i}&quot;].PutValue($&quot;Row{i}&quot;);
            //}

            //Cells A3, A4, A5 are visible and shouldn&apos;t be
            //The document behaves the way I would expect after I toggle the group manually
            worksheet1.Cells.GroupRows(1, 8, true);
            worksheet1.Cells.GroupRows(6, 8, true);
            worksheet1.Cells.GroupRows(2, 4, false);

            ////Order of the GroupRows calls seems to matter as well as this produces a different result
            ////Cells A3, A4, A5 should be visible but are hidden after uncollapsing the outer group manually in excel
            worksheet2.Cells.GroupRows(6, 8, true);
            worksheet2.Cells.GroupRows(2, 4, false);
            worksheet2.Cells.GroupRows(1, 9, true);

            ////Another modification on the same values
            ////The inner groups should be collapsed, but aren&apos;t when I set the outer group to be visible
            worksheet3.Cells.GroupRows(6, 8, true);
            worksheet3.Cells.GroupRows(2, 4, true);
            worksheet3.Cells.GroupRows(1, 8, false);

            ////Moving the outer row call first works
            worksheet4.Cells.GroupRows(1, 8, false);
            worksheet4.Cells.GroupRows(6, 8, true);
            worksheet4.Cells.GroupRows(2, 4, true);
            Util.SaveManCheck(workbook, &quot;Shape&quot;, &quot;CellsNet45555.xlsx&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

Groups rows.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | The first row index to be grouped. |
| lastIndex | Int32 | The last row index to be grouped. |

### Examples

```csharp
// Called: cells.GroupRows(1048576, 2);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Int32_()
        {
            caseName = &quot;testGroupRows_Exception_003&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.GroupRows(1048576, 2);
            string msg = message + &quot;cells.GroupRows(1048576, 2)&quot;;
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


