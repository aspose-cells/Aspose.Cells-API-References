---
title: Worksheet.FreezePanes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Freezes panes at the specified cell in the worksheet
type: docs
url: /net/aspose.cells/worksheet/freezepanes/
---
## FreezePanes(int, int, int, int) {#freezepanes}

Freezes panes at the specified cell in the worksheet.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| column | Int32 | Column index. |
| freezedRows | Int32 | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Int32 | Number of visible columns in left pane, no more than column index. |

### Remarks

Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.

The first two parameters specify the froze position and the last two parameters specify the area frozen on the left top pane.

### Examples

```csharp
// Called: wb.Worksheets[&amp;quot;ANT_ABS_ABS4_KPIs&amp;quot;].FreezePanes(r, c, rs, cs);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet42890.xls&quot;);
            int r, c, rs, cs;
            wb.Worksheets[&quot;ANT_ABS_ABS4_KPIs&quot;].GetFreezedPanes(out r, out c, out rs, out cs);
            wb.Worksheets[&quot;ANT_ABS_ABS4_KPIs&quot;].FreezePanes(r, c, rs, cs); 
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## FreezePanes(string, int, int) {#freezepanes_1}

Freezes panes at the specified cell in the worksheet.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| freezedRows | Int32 | Number of visible rows in top pane, no more than row index. |
| freezedColumns | Int32 | Number of visible columns in left pane, no more than column index. |

### Remarks

Row index and column index cannot all be zero. Number of rows and number of columns also cannot all be zero.

### Examples

```csharp
// Called: worksheet.FreezePanes(&amp;quot;C3&amp;quot;, 3, 3);
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Set worksheet properties
            worksheet.Name = &quot;DemoSheet&quot;;
            worksheet.IsGridlinesVisible = true;
            worksheet.IsRowColumnHeadersVisible = true;
            worksheet.DisplayZeros = true;
            worksheet.DisplayRightToLeft = false;
            worksheet.IsOutlineShown = true;
            worksheet.IsSelected = true;
            worksheet.FirstVisibleRow = 0;
            worksheet.FirstVisibleColumn = 0;
            worksheet.Zoom = 100;
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsPageBreakPreview = false;
            worksheet.IsRulerVisible = true;
            worksheet.TabColor = System.Drawing.Color.Blue;
            worksheet.CodeName = &quot;Sheet1&quot;;
            worksheet.ActiveCell = &quot;A1&quot;;

            // Add a hyperlink in Cell A1
            worksheet.Hyperlinks.Add(&quot;A1&quot;, 1, 1, &quot;http://www.aspose.com&quot;);

            // Freeze panes at &quot;C3&quot; with 3 row and 3 column
            worksheet.FreezePanes(&quot;C3&quot;, 3, 3);

            // Add a conditional formatting rule
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Setting properties for AboveAverage rule
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Save the workbook
            workbook.Save(&quot;WorksheetExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


