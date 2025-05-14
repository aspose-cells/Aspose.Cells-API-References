---
title: StyleFlag.Borders
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. All borders settings will be applied
type: docs
url: /net/aspose.cells/styleflag/borders/
---
## StyleFlag.Borders property

All borders settings will be applied.

```csharp
public bool Borders { get; set; }
```

### Examples

```csharp
// Called: sflag.Borders = true;
public void StyleFlag_Property_Borders()
{
    caseName = "testApplyStyle_002";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Style style = getStyle(workbook);
    StyleFlag sflag = new StyleFlag();
    sflag.Borders = true;

    cells.ApplyStyle(style, sflag);

    checkApplyStyle_001(workbook);
    workbook.Save(Constants.destPath + "testApplyStyle.xlsx");
    workbook = new Workbook(Constants.destPath + "testApplyStyle.xlsx");
    checkApplyStyle_001(workbook);
    workbook.Save(Constants.destPath + "testApplyStyle.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testApplyStyle.xml");
    workbook.Save(Constants.destPath + "testApplyStyle.xls");
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


