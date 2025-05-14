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
// Called: worksheet.FreezePanes(3, 3, 3, 3);
public void Worksheet_Method_FreezePanes()
{

    Workbook workbook = new Workbook();
    Worksheet worksheet = workbook.Worksheets[0];

    worksheet.FreezePanes(3, 3, 3, 3);
    byte paneId = 0;
   // int row, column, rows, columns;
    //Aspose.Cells.NUnitTest1.GetPaneInfo(worksheet, out paneId, out row, out column, out rows, out columns);

    Assert.AreEqual(paneId,0);
    workbook.Save(Constants.destPath + "example.xls");
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
// Called: worksheet.FreezePanes("C3", 3, 3);
public static void Worksheet_Method_FreezePanes()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Set worksheet properties
            worksheet.Name = "DemoSheet";
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
            worksheet.CodeName = "Sheet1";
            worksheet.ActiveCell = "A1";

            // Add a hyperlink in Cell A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Freeze panes at "C3" with 3 row and 3 column
            worksheet.FreezePanes("C3", 3, 3);

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
            workbook.Save("WorksheetExample.xlsx");

            return;
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


