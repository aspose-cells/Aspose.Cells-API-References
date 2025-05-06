---
title: FormatCondition.Formula2
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Gets and sets the value or expression associated with conditional formatting
type: docs
url: /net/aspose.cells/formatcondition/formula2/
---
## FormatCondition.Formula2 property

Gets and sets the value or expression associated with conditional formatting.

```csharp
public string Formula2 { get; set; }
```

### Remarks

Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".

### Examples

```csharp
// Called: testAreEqual(&amp;quot;10&amp;quot;, fc.Formula2, caseName);
private void Property_Formula2(Workbook workbook)
        { 
            Worksheet sheet = workbook.Worksheets[&quot;sheetDest&quot;];
            ConditionalFormattingCollection conformattings = sheet.ConditionalFormattings;
            testAreEqual(3, conformattings.Count, caseName);
            for (int i = 0; i &lt; conformattings.Count; i++)
            {
                FormatConditionCollection fcArr = conformattings[i];
                testAreEqual(1, fcArr.RangeCount, caseName);
                CellArea cellarea = (CellArea)fcArr.GetCellArea(0);
                if (cellarea.StartRow == 4 &amp;&amp; cellarea.StartColumn == 5 &amp;&amp;
                    cellarea.EndRow == 8 &amp;&amp; cellarea.EndColumn == 5)
                {
                    testAreEqual(1, fcArr.Count, caseName);
                    FormatCondition fc = fcArr[0];
                    testAreEqual(FormatConditionType.CellValue, fc.Type, caseName);
                    testAreEqual(OperatorType.Between, fc.Operator, caseName);
                    testAreEqual(&quot;0&quot;, fc.Formula1, caseName);
                    testAreEqual(&quot;10&quot;, fc.Formula2, caseName);
                    Style style = fc.Style;
                    testequals(Color.FromArgb(255, 204, 0), style.Borders[BorderType.TopBorder].Color, caseName);
                    testAreEqual(CellBorderType.Hair, style.Borders[BorderType.TopBorder].LineStyle, caseName);
                    testequals(Color.FromArgb(0, 255, 0), style.Borders[BorderType.LeftBorder].Color, caseName);
                    testAreEqual(CellBorderType.DashDotDot, style.Borders[BorderType.LeftBorder].LineStyle, caseName);
                    testequals(Color.FromArgb(255, 0, 0), style.Borders[BorderType.RightBorder].Color, caseName);
                    testAreEqual(CellBorderType.DashDot, style.Borders[BorderType.RightBorder].LineStyle, caseName);
                    testequals(Color.FromArgb(0, 0, 128), style.Borders[BorderType.BottomBorder].Color, caseName);
                    testAreEqual(CellBorderType.Thin, style.Borders[BorderType.BottomBorder].LineStyle, caseName);
                    testAreEqual(BackgroundType.DiagonalCrosshatch, style.Pattern, caseName);
                    testequals(Color.Red, style.BackgroundColor, caseName);
                    testequals(Color.FromArgb(51, 102, 255), style.ForegroundColor, caseName);
                }
                else if (cellarea.StartRow == 15 &amp;&amp; cellarea.StartColumn == 5 &amp;&amp;
                    cellarea.EndRow == 20 &amp;&amp; cellarea.EndColumn == 5)
                {
                    testAreEqual(1, fcArr.Count, caseName);
                    FormatCondition fc = fcArr[0];
                    testAreEqual(FormatConditionType.CellValue, fc.Type, caseName);
                    testAreEqual(OperatorType.Between, fc.Operator, caseName);
                    testAreEqual(&quot;0&quot;, fc.Formula1, caseName);
                    testAreEqual(&quot;1&quot;, fc.Formula2, caseName);
                    Style style = fc.Style;
                    testequals(Color.Red, style.Font.Color, caseName);
                    testAreEqual(&quot;����&quot;, style.Font.Name, caseName);
                    testAreEqual(12, style.Font.Size, caseName);
                    testAreEqual(FontUnderlineType.Single, style.Font.Underline, caseName);
                    testequals(Color.FromArgb(255, 0, 255), style.Borders[BorderType.TopBorder].Color, caseName);
                    testAreEqual(CellBorderType.Dashed, style.Borders[BorderType.TopBorder].LineStyle, caseName);
                    testequals(Color.FromArgb(255, 0, 255), style.Borders[BorderType.LeftBorder].Color, caseName);
                    testAreEqual(CellBorderType.Dashed, style.Borders[BorderType.LeftBorder].LineStyle, caseName);
                    testequals(Color.FromArgb(255, 0, 255), style.Borders[BorderType.RightBorder].Color, caseName);
                    testAreEqual(CellBorderType.Dashed, style.Borders[BorderType.RightBorder].LineStyle, caseName);
                    testequals(Color.FromArgb(255, 0, 255), style.Borders[BorderType.BottomBorder].Color, caseName);
                    testAreEqual(CellBorderType.Dashed, style.Borders[BorderType.BottomBorder].LineStyle, caseName);
                }
                else if (cellarea.StartRow == 31 &amp;&amp; cellarea.StartColumn == 5 &amp;&amp;
                 cellarea.EndRow == 31 &amp;&amp; cellarea.EndColumn == 5)
                {
                    testAreEqual(1, fcArr.Count, caseName);
                    FormatCondition fc = fcArr[0];
                    testAreEqual(FormatConditionType.CellValue, fc.Type, caseName);
                    testAreEqual(OperatorType.Between, fc.Operator, caseName);
                    testAreEqual(&quot;0&quot;, fc.Formula1, caseName);
                    testAreEqual(&quot;1&quot;, fc.Formula2, caseName);
                    Style style = fc.Style;
                    testequals(Color.Blue, style.BackgroundColor, caseName);
                }
            }            
            //WorkbookCompare.ConditionalFormattingsTest.equals(sheetSrc.ConditionalFormattings, sheetDest.ConditionalFormattings, caseName);
        }
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


