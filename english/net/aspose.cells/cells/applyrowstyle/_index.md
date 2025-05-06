---
title: Cells.ApplyRowStyle
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Applies formats for a whole row
type: docs
url: /net/aspose.cells/cells/applyrowstyle/
---
## Cells.ApplyRowStyle method

Applies formats for a whole row.

```csharp
public void ApplyRowStyle(int row, Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: cells.ApplyRowStyle(1, style, sflag);
[Test]
        public void Method_StyleFlag_()
        {
            caseName = &quot;testApplyRowStyle_001&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = getStyle(workbook);
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;
            cells.ApplyRowStyle(1, style, sflag);            

            checkApplyRowStyle_001(workbook);
            workbook.Save(Constants.destPath + &quot;testApplyRowStyle.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testApplyRowStyle.xls&quot;);
            checkApplyRowStyle_001(workbook);
            workbook.Save(Constants.destPath + &quot;testApplyRowStyle.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testApplyRowStyle.xlsx&quot;);
            checkApplyRowStyle_001(workbook);
            workbook.Save(Constants.destPath + &quot;testApplyRowStyle.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testApplyRowStyle.xml&quot;);
            checkApplyRowStyle_001(workbook);
            workbook.Save(Constants.destPath + &quot;testApplyRowStyle.xls&quot;);  
        }
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


