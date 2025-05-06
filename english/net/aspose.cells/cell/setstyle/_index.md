---
title: Cell.SetStyle
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Sets the cell style
type: docs
url: /net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

Sets the cell style.

```csharp
public void SetStyle(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |

### Remarks

If the border settings are changed, the border of adjust cells will be updated too.

### Examples

```csharp
// Called: cells[1048575, 0].SetStyle(style);
[Test]
        public void Method_Style_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Style style = wb.CreateStyle();
            style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Green);
            cells[1048575, 0].SetStyle(style);
            Assert.AreEqual(BackgroundType.Solid, cells[1048575, 0].GetStyle().Pattern, &quot;Before insert&quot;);
            cells.InsertRows(0, 2);
            Assert.AreEqual(BackgroundType.None, cells[1048575, 0].GetStyle().Pattern, &quot;After insert&quot;);
            cells[1048575, 0].PutValue(1);
            bool fail = false;
            try
            {
                cells.InsertRows(0, 2);
                fail = true;
            }
            catch (CellsException e)
            {
                Assert.AreEqual(ExceptionType.Limitation, e.Code, &quot;Exception type of invalid insert operation&quot;);
            }
            if (fail)
            {
                Assert.Fail(&quot;Insert operation should not be allowed when there are cells with data to be moved out of sheet&quot;);
            }
        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, bool) {#setstyle_2}

Apply the changed property of style to the cell.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | Boolean | True, only overwriting formatting which is explicitly set. |

### Examples

```csharp
// Called: cell.SetStyle(style, true);
public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(USBankConstants.sourcePath + &quot;Styles.xlsx&quot;);

            Style style = workbook.GetNamedStyle(&quot;SecondaryStyle_Locked&quot;);
            Cell cell = workbook.Worksheets[0].Cells[&quot;B2&quot;];
            cell.SetStyle(style, true);

            style = workbook.GetNamedStyle(&quot;SecondaryStyle_LockedHidden&quot;);
            cell = workbook.Worksheets[0].Cells[&quot;B3&quot;];
            cell.SetStyle(style, true);

            string output = USBankConstants.resultPath + &quot;Styles_result.xlsx&quot;;
            workbook.Save(output);
           
        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, StyleFlag) {#setstyle_1}

Apply the cell style based on flags.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| flag | StyleFlag | The style flag. |

### Examples

```csharp
// Called: sheet.Cells[k, 0].SetStyle(headerStyle, styleFlagHeader);
protected static void Method_StyleFlag_(Workbook book)
        {
            for (int i = 0; i &lt; book.Worksheets.Count; i++)
            {
                Worksheet sheet = book.Worksheets[i];
                StyleFlag styleFlagHeader = new StyleFlag();
                styleFlagHeader.All = true;
                Style headerStyle = book.CreateStyle();
                headerStyle.ForegroundColor = System.Drawing.Color.FromArgb(255, 238, 238, 238);
                headerStyle.Pattern = BackgroundType.Solid;
                headerStyle.Font.IsBold = true;
                headerStyle.VerticalAlignment = TextAlignmentType.Center;
                headerStyle.HorizontalAlignment = TextAlignmentType.Center;
                headerStyle.SetBorder(BorderType.LeftBorder, CellBorderType.Thin,
                        System.Drawing.Color.FromArgb(255, 204, 204, 204));
                headerStyle.SetBorder(BorderType.RightBorder, CellBorderType.Thin,
                        System.Drawing.Color.FromArgb(255, 204, 204, 204));
                headerStyle.SetBorder(BorderType.BottomBorder,
                        CellBorderType.Thin, System.Drawing.Color.FromArgb(255, 204, 204, 204));
                headerStyle.SetBorder(BorderType.TopBorder, CellBorderType.Thin,
                        System.Drawing.Color.FromArgb(255, 204, 204, 204));

                int maxRow = sheet.Cells.MaxRow;
                int maxCol = sheet.Cells.MaxColumn;
                for (int k = 0; k &lt;= maxRow; k++)
                {
                    sheet.Cells[k, 0].SetStyle(headerStyle, styleFlagHeader);
                }
                for (int j = 0; j &lt;= maxCol; j++)
                {
                    sheet.Cells[0, j].SetStyle(headerStyle, styleFlagHeader);
                }
            }
        }
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


