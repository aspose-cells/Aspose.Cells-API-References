---
title: DataSorter.Sort
second_title: Aspose.Cells for .NET API Reference
description: DataSorter method. Sorts the data of the area
type: docs
url: /net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Sorts the data of the area.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| startRow | Int32 | The start row of the area. |
| startColumn | Int32 | The start column of the area. |
| endRow | Int32 | The end row of the area. |
| endColumn | Int32 | The end column of the area. |

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### Examples

```csharp
// Called: sorter.Sort(cells, 0, 0, 999, 1);
[Test]
        public void Method_Int32_() //Cannot reproduce user&apos;s issue, no matter using shared formula or normal formulas.
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].SetSharedFormula(&quot;=COUNTIF($B$1:$B1,B1)&quot;, 1000, 1);
            for (int i = 0; i &lt; 1000; i++)
            {
                cells[i, 1].PutValue(i);
                //cells[i, 0].Formula = &quot;=COUNTIF($B$1:$B&quot; + (i + 1) + &quot;,B&quot; + (i + 1) + &quot;)&quot;;
                Assert.AreEqual(&quot;=COUNTIF($B$1:$B&quot; + (i + 1) + &quot;,B&quot; + (i + 1) + &quot;)&quot;, cells[i, 0].Formula);
            }
            cells[20, 1].PutValue(800);
            cells[800, 1].PutValue(20);
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(1, SortOrder.Ascending);
            sorter.Sort(cells, 0, 0, 999, 1);
            for (int i = 0; i &lt; 1000; i++)
            {
                Assert.AreEqual(&quot;=COUNTIF($B$1:$B&quot; + (i + 1) + &quot;,B&quot; + (i + 1) + &quot;)&quot;,
                    cells[i, 0].Formula, &quot;A&quot; + (i + 1));
                Assert.AreEqual(i, cells[i, 1].IntValue, &quot;A&quot; + (i + 1));
            }
        }
```

### See Also

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Sort the data of the area.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| area | CellArea | The area needed to sort |

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### Examples

```csharp
// Called: sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 9, 0));
[Test]
        public void Method_CellArea_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            for (int i = 0; i &lt; 10; i++)
            {
                cells[i, 0].PutValue(i);
            }
            Style style = wb.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            cells[4, 0].SetStyle(style);
            cells[8, 0].SetStyle(style);
            style.ForegroundColor = Color.Blue;
            cells[6, 0].SetStyle(style);
            cells[9, 0].SetStyle(style);
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.Add(CellArea.CreateCellArea(0, 0, 3, 0), FormatConditionType.CellValue,
                OperatorType.Between, &quot;1&quot;, &quot;2&quot;);
            FormatCondition fc = fcc[0];
            fc.Style.Pattern = BackgroundType.Solid;
            fc.Style.BackgroundColor = Color.Blue;
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOnType.CellColor, SortOrder.Ascending, Color.Blue);
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 9, 0));
            int[] vs = new int[] { 1, 2, 6, 9, 0, 3, 4, 5, 7, 8, };
            for (int i = 0; i &lt; vs.Length; i++)
            {
                Assert.AreEqual(vs[i], cells[i, 0].IntValue, &quot;A&quot; + (i + 1));
            }
        }
```

### See Also

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Sort the data in the range.

```csharp
public int[] Sort()
```

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### Examples

```csharp
// Called: lo.AutoFilter.Sorter.Sort();
private static void Method_Sort(Workbook wb)
        {
            #region UPDATE pivot tables
            //Before the populated excel file is saved, calculate all pivot tables and charts.
            //Calculate formula has to be called before filtering to allow filters on calculated fields.
            wb.CalculateFormula();

            foreach (Worksheet sheet in wb.Worksheets)
            {
                sheet.CalculateFormula(new CalculationOptions(), true);

                foreach (Aspose.Cells.Tables.ListObject lo in sheet.ListObjects)
                {
                    //A sort needs to be done after all tables have been filled as some tables may be sorted using a formula column referencing other tables.
                    lo.AutoFilter.Sorter.Sort();
                    sheet.CalculateFormula(new CalculationOptions(), true);
                    lo.AutoFilter.Refresh();
                }
            }
            wb.CalculateFormula();

            foreach (Worksheet sheet in wb.Worksheets)
            {
                foreach (Aspose.Cells.Pivot.PivotTable t in sheet.PivotTables)
                {
                    if (t.DataSource != null)
                    {
                        t.RefreshData();
                        //Range needs to be calculated before data is calculated to ensure that the record count is accounted for by the pivot table refresh.
                        t.CalculateRange();
                        t.CalculateData();
                        t.RefreshDataOnOpeningFile = true;
                    }
                }
            }
            wb.CalculateFormula();
            #endregion

            #region UPDATE all charts in the workbook
            foreach (Worksheet sh in wb.Worksheets)
            {
                if (sh.Charts.Count &gt; 0)
                {
                    foreach (Chart chart in sh.Charts)
                    {
                        if (chart.PivotSource != null)
                        {
                            //Line is important to update pivot charts.
                            chart.RefreshPivotData();
                        }
                    }
                }
            }
            #endregion

            #region Row Height Handling code
            //Make sure that all rows allows enough height to display data in each cells (for word wrapped cells).
            foreach (Worksheet sheet in wb.Worksheets)
            {
                AutoFitterOptions fitter = new AutoFitterOptions();
                fitter.IgnoreHidden = true;
                sheet.AutoFitRows(fitter);                
            }
            #endregion
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


