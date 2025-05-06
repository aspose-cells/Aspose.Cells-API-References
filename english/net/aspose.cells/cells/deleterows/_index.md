---
title: Cells.DeleteRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Deletes multiple rows
type: docs
url: /net/aspose.cells/cells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Deletes multiple rows.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | The first row index to be deleted. |
| totalRows | Int32 | Count of rows to be deleted. |

### Remarks

If the deleted range contains the top part(not whole) of the table(ListObject), the ranged could not be deleted and nothing will be done. It works in the same way with MS Excel.

### Examples

```csharp
// Called: cells.DeleteRows(1, 3);
[Test]
        public void Method_Int32_()
        {
            caseName = &quot;testDeleteRows_004&quot;;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Cells\\deleteColumn_002.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.DeleteRows(1, 3);

            checkDeleteRows_004(workbook);
            workbook.Save(Constants.destPath + &quot;testDeleteRows.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testDeleteRows.xls&quot;);
            checkDeleteRows_004(workbook);
            workbook.Save(Constants.destPath + &quot;testDeleteRows.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testDeleteRows.xlsx&quot;);
            checkDeleteRows_004(workbook);
            workbook.Save(Constants.destPath + &quot;testDeleteRows.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testDeleteRows.xml&quot;);
            checkDeleteRows_004(workbook);
            workbook.Save(Constants.destPath + &quot;testDeleteRows.xls&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_2}

Deletes multiple rows in the worksheet.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index of the first row to be deleted. |
| totalRows | Int32 | Count of rows to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |

### Examples

```csharp
// Called: cells.DeleteRows(0, 1, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            int v0 = wb.DefaultStyle.Font.Size;
            int v1 = v0 + 5;
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 10; i++)
            {
                for (int j = 0; j &lt; 4; j++)
                {
                    cells[i, j].PutValue(true);
                }
            }
            ConditionalFormattingCollection cfc = wb.Worksheets[0].ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 4, 2));
            FormatCondition fc = fcc[fcc.AddCondition(FormatConditionType.Expression)];
            string[] fmls = new string[] { &quot;=$A1=TRUE&quot; };
            fc.Formula1 = fmls[0];
            fc.Style.Font.Size = v1;
            for (int i = 0; i &lt; 10; i++)
            {
                for (int j = 0; j &lt; 4; j++)
                {
                    bool applied = j &lt; 3 &amp;&amp; i &lt; 5;
                    CheckCellFormatConditions(cells[i, j], applied ? v1 : v0, applied ? fmls : null,
                        &quot;With original conditional formatting,&quot;);
                }
            }
            cells.DeleteRows(0, 1, true);
            CheckEmptyAppliedRange(cfc, &quot;After deleting row,&quot;);
            for (int i = 0; i &lt; 10; i++)
            {
                for (int j = 0; j &lt; 4; j++)
                {
                    bool applied = j &lt; 3 &amp;&amp; i &lt; 4;
                    CheckCellFormatConditions(cells[i, j], applied ? v1 : v0, applied ? fmls : null, &quot;After deleting row,&quot;);
                }
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, DeleteOptions) {#deleterows_1}

Deletes multiple rows in the worksheet.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, DeleteOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index of the first row to be deleted. |
| totalRows | Int32 | Count of rows to be deleted. |
| options | DeleteOptions | Options for the deleting operation |

### Examples

```csharp
// Called: cells.DeleteRows(6, 3, dopts);
[Test]
        public void Method_DeleteOptions_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets.Add(&quot;Sheet2&quot;).Cells;
            cells[0, 0].Formula = &quot;=Sheet1!A10&quot;;
            cells[0, 1].Formula = &quot;=Sheet1!A5&quot;;
            cells[0, 2].Formula = &quot;=A10&quot;;
            cells[0, 3].Formula = &quot;=A5&quot;;
            cells = wb.Worksheets[0].Cells;
            cells[0, 0].Formula = &quot;=A10&quot;;
            cells[0, 1].Formula = &quot;=A5&quot;;

            DeleteOptions dopts = new DeleteOptions();
            HashSet&lt;int&gt; changed = new HashSet&lt;int&gt;();
            dopts.FormulaChangeMonitor = new MyCellChangeMonitor(changed);
            dopts.UpdateReference = true;
            cells.DeleteRows(6, 3, dopts);
            Assert.AreEqual(2, changed.Count, &quot;Delete: Total changed cells&quot;);
            if (!changed.Contains(0))
            {
                Assert.Fail(&quot;Delete: Monitor should find Sheet1!A1 has been changed.&quot;);
            }
            if (!changed.Contains(1 &lt;&lt; 24))
            {
                Assert.Fail(&quot;Delete: Monitor should find Sheet2!A1 has been changed.&quot;);
            }
            changed.Clear();
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            iopts.FormulaChangeMonitor = new MyCellChangeMonitor(changed);
            cells.InsertRows(6, 3, iopts);
            Assert.AreEqual(2, changed.Count, &quot;Insert: Total changed cells&quot;);
            if (!changed.Contains(0))
            {
                Assert.Fail(&quot;Insert: Monitor should find Sheet1!A1 has been changed.&quot;);
            }
            if (!changed.Contains(1 &lt;&lt; 24))
            {
                Assert.Fail(&quot;Insert: Monitor should find Sheet2!A1 has been changed.&quot;);
            }
        }
```

### See Also

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


