---
title: Cell.GetDisplayStyle
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the display style of this cell
type: docs
url: /net/aspose.cells/cell/getdisplaystyle/
---
## GetDisplayStyle() {#getdisplaystyle}

Gets the display style of this cell.

```csharp
public Style GetDisplayStyle()
```

### Return Value

display style of this cell

### Remarks

Same with using SideBorders for `GetDisplayStyle`. That is, this method will check and adjust top/bottom/left/right borders of this cell according to the style([`GetStyle`](../getstyle/)) of its adjacent cells, but do not check the merged cells, and do not check the display style of adjacent cells.

### Examples

```csharp
// Called: Color backgroundColor = cell.GetDisplayStyle().ForegroundColor;
[Test]
        public void Method_GetDisplayStyle()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CellsJava44100.xlsx");
            workbook.Worksheets.RefreshPivotTables();
            Cell cell = workbook.Worksheets[0].Cells["I6"];
            Color backgroundColor = cell.GetDisplayStyle().ForegroundColor;
           AssertHelper.AreEqual(Color.FromArgb(251,229, 214), backgroundColor);
            Color backgroundColor1 = cell.GetDisplayStyle().BackgroundColor;
            workbook.Save(Constants.PivotTableDestPath + "CellsJava44100.xlsx");

        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(bool) {#getdisplaystyle_2}

Gets the display style of this cell.

```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| includeMergedBorders | Boolean | Indicates whether checking borders of merged cells. |

### Return Value

display style of this cell

### Remarks

If the specified flag is false, then it is same with `GetDisplayStyle`. Otherwise it is same with using SideBorders&#x7C;DynamicStyleBorders for `GetDisplayStyle`.

### Examples

```csharp
// Called: Style style = cell.GetDisplayStyle(true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava42716.xlsx");

            Cell cell = workbook.Worksheets[0].Cells["B2"];
            Style style = cell.GetDisplayStyle(true);
            Assert.AreEqual(style.Borders[BorderType.RightBorder].LineStyle,CellBorderType.Thin);

        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(BorderType) {#getdisplaystyle_1}

Gets the display style of this cell.

```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| adjacentBorders | BorderType | Indicates which borders need to be checked and adjusted according to the borders of adjacent cells. |

### Return Value

display style of this cell

### Remarks

If this cell is also affected by other settings such as conditional formatting, list objects, etc., then the display style may be different from [`GetStyle`](../getstyle/). For flags of adjusting borders according to adjacent cells, TopBorder/BottomBorder /LeftBorder/RightBorder denote whether check and combine the bottom/top/right/left borders of the left/right/top/bottom cells adjacent to this one. For performance and compatibility consideration, some enums are used to denote some special operations: Horizontal/Vertical denote whether check and combine the bottom/right border of merged cells to this one. Diagonal(that is, both DiagonalUpBorder and DiagonalDownBorder have been set) denotes check and combine borders from the display style of adjacent cells. Please note, checking borders/styles of adjacent cells, especially the display styles, is time-consumed process. If there is no need to get the borders for the returned style, using None to disable the process of adjacent cells will give better performance. When getting borders of adjacent cells from styles defined on those cells only(without setting Diagonal), the performance also may be better because checking the display style of one cell is time-consumed too.

### Examples

```csharp
// Called: if (cells[r, 0].GetDisplayStyle(BorderType.None).ForegroundArgbColor != argbs[r % 10])
[Test]
        public void Method_BorderType_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            for (int i = 0; i < 100000; i++)
            {
                cells[i, 0].PutValue(i % 10);
            }
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 1048575, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);
            int[] argbs = new int[]
            {
                //0xFFF8696B, 0xFFF98570, 0xFFFBA276, 0xFFFCBF7B, 0xFFFEDC81, 0xFFEDE582, 0xFFCADB80, 0xFFA8D17E, 0xFF85C77C, 0xFF63BE7B,
                -497301, -424592, -286090, -213125, -74623, -1186430, -3482752, -5713538, -8009860, -10240389,
            };

            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            TimePerformance monitor = new TimePerformance(70);
            monitor.StartPerfTest();
            Random random = new Random();
            for (int i = 0; i < 5000; i++)
            {
                int r = (int)(100000 * random.NextDouble());
                if (cells[r, 0].GetDisplayStyle(BorderType.None).ForegroundArgbColor != argbs[r % 10])
                {
                    Assert.Fail("A" + (r + 1) + " expected color should be "
                        + argbs[r % 10].ToString("X") + " but was "
                        + cells[r, 0].GetDisplayStyle().ForegroundArgbColor.ToString("X"));
                }
            }
            monitor.FinishPerfTest("Using access cache for conditional formattings with type of ColorScale");

            sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
```

### See Also

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


