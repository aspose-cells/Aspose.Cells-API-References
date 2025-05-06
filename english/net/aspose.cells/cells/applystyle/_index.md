---
title: Cells.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Applies formats for a whole worksheet
type: docs
url: /net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

Applies formats for a whole worksheet.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: cells.ApplyStyle(style, sflag);
[Test]
        public void Method_StyleFlag_()
        {
            caseName = &quot;testApplyStyle_001&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = getStyle(workbook);
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;

            cells.ApplyStyle(style, sflag);

            checkApplyStyle_001(workbook);
            workbook.Save(Constants.destPath + &quot;testApplyStyle.xls&quot;);            
            workbook = new Workbook(Constants.destPath + &quot;testApplyStyle.xls&quot;);
            checkApplyStyle_001(workbook);
            workbook.Save(Constants.destPath + &quot;testApplyStyle.xlsx&quot;);            
            workbook = new Workbook(Constants.destPath + &quot;testApplyStyle.xlsx&quot;);
            checkApplyStyle_001(workbook);
            workbook.Save(Constants.destPath + &quot;testApplyStyle.xml&quot;, SaveFormat.SpreadsheetML);            
            workbook = new Workbook(Constants.destPath + &quot;testApplyStyle.xml&quot;);
            checkApplyStyle_001(workbook);
            workbook.Save(Constants.destPath + &quot;testApplyStyle.xls&quot;);           

            
            //for (IEnumerator ie = cells.GetEnumerator(); ie.MoveNext; )
            //{
            //    Cell cell = (Cell)ie.Current;
            //}
            
            //for (int row = 0; row &lt; 65536; row++)
            //{               
            //    for (int col = 0; col &lt; 256; col++)
            //    {
            //        Cell cell = cells.GetCellOrNull(row, col);
            //        if (cell != null)
            //        {
            //            Style styleDest = cell.GetStyle();
            //            testequals(Color.Red, styleDest.Borders[BorderType.TopBorder].Color, caseName);
            //            testAreEqual(CellBorderType.Dashed, styleDest.Borders[BorderType.TopBorder].LineStyle, caseName);
            //            testequals(Color.Blue, styleDest.Borders[BorderType.LeftBorder].Color, caseName);
            //            testAreEqual(CellBorderType.Dotted, styleDest.Borders[BorderType.LeftBorder].LineStyle, caseName);
            //            testequals(Color.Green, styleDest.Borders[BorderType.RightBorder].Color, caseName);
            //            testAreEqual(CellBorderType.Double, styleDest.Borders[BorderType.RightBorder].LineStyle, caseName);
            //        }
            //    }
            //}
            //workbook.Save(@&quot;D:\test.xls&quot;);
        }
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


