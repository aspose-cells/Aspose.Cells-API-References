---
title: Cells.ApplyColumnStyle
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Applies formats for a whole column
type: docs
url: /net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

Applies formats for a whole column.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index. |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: cells.ApplyColumnStyle(1, style, sflag);
public void Cells_Method_ApplyColumnStyle()
{
    caseName = "testApplyColumnStyle_001";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Style style = getStyle(workbook);
    StyleFlag sflag = new StyleFlag();
    sflag.Borders = true;
    cells.ApplyColumnStyle(1, style, sflag);

    checkApplyColumnStyle_001(workbook);
    workbook.Save(Constants.destPath + "testApplyColumnStyle.xls");
    workbook = new Workbook(Constants.destPath + "testApplyColumnStyle.xls");
    checkApplyColumnStyle_001(workbook);
    workbook.Save(Constants.destPath + "testApplyColumnStyle.xlsx");
    workbook = new Workbook(Constants.destPath + "testApplyColumnStyle.xlsx");
    checkApplyColumnStyle_001(workbook);
    workbook.Save(Constants.destPath + "testApplyColumnStyle.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testApplyColumnStyle.xml");
    checkApplyColumnStyle_001(workbook);
    workbook.Save(Constants.destPath + "testApplyColumnStyle.xls");              
}
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


