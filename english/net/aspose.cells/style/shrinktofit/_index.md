---
title: Style.ShrinkToFit
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents if text automatically shrinks to fit in the available column width
type: docs
url: /net/aspose.cells/style/shrinktofit/
---
## Style.ShrinkToFit property

Represents if text automatically shrinks to fit in the available column width.

```csharp
public bool ShrinkToFit { get; set; }
```

### Examples

```csharp
// Called: style.ShrinkToFit = true;
public void Style_Property_ShrinkToFit()
{
    caseName = "testShrinkToFit_002";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Style style = cells[0, 0].GetStyle();
    style.ShrinkToFit = true;
    cells[0, 0].SetStyle(style);
    testAreEqual(true, cells[0, 0].GetStyle().ShrinkToFit, caseName);

    checkShrinkToFit_002(workbook);
    workbook.Save(Constants.destPath + "testShrinkToFit.xls");
    workbook = new Workbook(Constants.destPath + "testShrinkToFit.xls");
    checkShrinkToFit_002(workbook);
    workbook.Save(Constants.destPath + "testRotation.xlsx");
    workbook = new Workbook(Constants.destPath + "testRotation.xlsx");
    checkShrinkToFit_002(workbook);
    workbook.Save(Constants.destPath + "testRotation.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testRotation.xml");
    checkShrinkToFit_002(workbook);
    workbook.Save(Constants.destPath + "testShrinkToFit.xls");
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


