---
title: PivotTable.HasBlankRows
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows
type: docs
url: /net/aspose.cells.pivot/pivottable/hasblankrows/
---
## PivotTable.HasBlankRows property

Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.

```csharp
public bool HasBlankRows { get; set; }
```

### Examples

```csharp
// Called: pivotTable.HasBlankRows = false;
[Test]
        public void Property_HasBlankRows()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET42621And42703And42753And42752_&quot;;
            #region net42621
            Workbook workbook = new Workbook(filePath + &quot;Sample.xlsx&quot;);
            workbook.CalculateFormula();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.PivotTables[0].RefreshData();
            sheet.PivotTables[0].CalculateData();
            CellArea[] areas = sheet.Cells.GetMergedAreas();
            bool b8b11 = false;
            bool b23c12 = false;
            CellArea area;
            for (int i = 0; i &lt; areas.Length; i++)
            {
                area = (CellArea)areas[i];
                if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B8&quot;, &quot;B11&quot;)))
                {
                    b8b11 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B12&quot;, &quot;C12&quot;)))
                {
                    b23c12 = true;
                }
            }
            Assert.AreEqual(b8b11 &amp;&amp; b23c12, true);
            Assert.AreEqual(sheet.Cells[&quot;B12&quot;].StringValue, &quot;Tổng&quot;);
            Assert.AreEqual(sheet.Cells[&quot;D8&quot;].StringValue, &quot;2&quot;);
            Assert.AreEqual(sheet.Cells[&quot;D9&quot;].StringValue, &quot;2&quot;);
            Assert.AreEqual(sheet.Cells[&quot;D11&quot;].StringValue, &quot;2&quot;);
            Assert.AreEqual(sheet.Cells[&quot;F7&quot;].StringValue, &quot;Tổng&quot;);
            workbook.Save(Constants.PivotTableDestPath + &quot;Net42621.pdf&quot;);
            #endregion

            #region net42703
            workbook = new Workbook(filePath + &quot;excelOutput.xlsx&quot;);
            foreach (Worksheet ws in workbook.Worksheets)
            {
                foreach (PivotTable pivotTable in ws.PivotTables)
                {
                    pivotTable.RefreshData();
                    pivotTable.CalculateData();
                    pivotTable.CalculateRange();

                    pivotTable.HasBlankRows = false;
                    pivotTable.PreserveFormatting = true;
                    pivotTable.MergeLabels = true;
                }
            }
            sheet = workbook.Worksheets[&quot;Report&quot;];
            areas = sheet.Cells.GetMergedAreas();
            bool b11b13 = false;
            bool b14b16 = false;
            bool b17d17 = false;
            for (int i = 0; i &lt; areas.Length; i++)
            {
                area = (CellArea)areas[i];
                if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B11&quot;, &quot;B13&quot;)))
                {
                    b11b13 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B14&quot;, &quot;B16&quot;)))
                {
                    b14b16 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B17&quot;, &quot;D17&quot;)))
                {
                    b17d17 = true;
                }
            }
            Assert.AreEqual(b11b13 &amp;&amp; b14b16 &amp;&amp; b17d17, true);
            Assert.AreEqual(sheet.Cells[&quot;B11&quot;].StringValue, &quot;2013&quot;);
            Assert.AreEqual(sheet.Cells[&quot;B14&quot;].StringValue, &quot;2014&quot;);
            Assert.AreEqual(sheet.Cells[&quot;B17&quot;].StringValue, &quot;Total&quot;);
            Cell f10 = sheet.Cells[&quot;F10&quot;];
            Cell f14 = sheet.Cells[&quot;F14&quot;];
            Assert.AreEqual(f10.StringValue, &quot;T4&quot;);
           AssertHelper.AreEqual(f10.GetStyle().ForegroundColor, Color.FromArgb(255, 142, 180, 227));
            Assert.AreEqual(f14.StringValue, &quot;55&quot;);
           AssertHelper.AreEqual(f14.GetStyle().ForegroundColor, Color.FromArgb(0, 255, 255, 255));
            workbook.Save(Constants.PivotTableDestPath + &quot;Net42703.pdf&quot;);
            #endregion

            #region net42752 and net42753
            workbook = new Workbook(filePath + &quot;MTR3100_Ouput.xlsx&quot;);
            foreach (Worksheet ws in workbook.Worksheets)
            {
                foreach (PivotTable pivotTable in ws.PivotTables)
                {
                    pivotTable.RefreshData();
                    pivotTable.CalculateData();
                    pivotTable.CalculateRange();

                    pivotTable.HasBlankRows = false;
                    pivotTable.PreserveFormatting = true;
                    pivotTable.MergeLabels = true;
                }
            }
            sheet = workbook.Worksheets[&quot;Report&quot;];
            areas = sheet.Cells.GetMergedAreas();
            bool b9b23 = false;
            bool b24e24 = false;
            bool b25e25 = false;
            bool c23e23 = false;
            bool c20e20 = false;
            bool g7g8 = false;
            bool i7i8 = false;
            bool c9c19 = false;
            bool c21c22 = false;
            bool d19e19 = false;
            for (int i = 0; i &lt; areas.Length; i++)
            {
                area = (CellArea)areas[i];
                if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B9&quot;, &quot;B23&quot;)))
                {
                    b9b23 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B24&quot;, &quot;E24&quot;)))
                {
                    b24e24 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;B25&quot;, &quot;E25&quot;)))
                {
                    b25e25 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;C23&quot;, &quot;E23&quot;)))
                {
                    c23e23 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;C20&quot;, &quot;E20&quot;)))
                {
                    c20e20 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;G7&quot;, &quot;G8&quot;)))
                {
                    g7g8 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;I7&quot;, &quot;I8&quot;)))
                {
                    i7i8 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;C9&quot;, &quot;C19&quot;)))
                {
                    c9c19 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;C21&quot;, &quot;C22&quot;)))
                {
                    c21c22 = true;
                }
                else if (IsEqualArea(area, CellArea.CreateCellArea(&quot;D19&quot;, &quot;E19&quot;)))
                {
                    d19e19 = true;
                }
            }
            Assert.AreEqual(b9b23 &amp;&amp; b24e24 &amp;&amp; b25e25 &amp;&amp; c23e23 &amp;&amp; c20e20 &amp;&amp; g7g8 &amp;&amp; i7i8 &amp;&amp; c9c19 &amp;&amp; c21c22 &amp;&amp; d19e19, true);
            Assert.AreEqual(sheet.Cells[&quot;C20&quot;].StringValue, &quot;1 Total&quot;);
            Assert.AreEqual(sheet.Cells[&quot;C23&quot;].StringValue, &quot;2 Total&quot;);
            Assert.AreEqual(sheet.Cells[&quot;B24&quot;].StringValue, &quot;2014 Total&quot;);
            Assert.AreEqual(sheet.Cells[&quot;B25&quot;].StringValue, &quot;Total&quot;);

            Assert.AreEqual(sheet.Cells[&quot;G7&quot;].StringValue, &quot;HKT06 Total&quot;);
            Assert.AreEqual(sheet.Cells[&quot;I7&quot;].StringValue, &quot;HKT03 Total&quot;);
            Assert.AreEqual(sheet.Cells[&quot;D19&quot;].StringValue, &quot;Children Total&quot;);
            Assert.AreEqual(sheet.Cells[&quot;C9&quot;].StringValue, &quot;1&quot;);
            Assert.AreEqual(sheet.Cells[&quot;C21&quot;].StringValue, &quot;2&quot;);
            workbook.Save(Constants.PivotTableDestPath + &quot;out42752and42753.pdf&quot;);
            #endregion
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


