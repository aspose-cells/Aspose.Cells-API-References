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
// Called: testAreEqual(true, cells[0, 0].GetStyle().ShrinkToFit, caseName);
[Test]
        public void Property_ShrinkToFit()
        {
            caseName = &quot;testShrinkToFit_002&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = cells[0, 0].GetStyle();
            style.ShrinkToFit = true;
            cells[0, 0].SetStyle(style);
            testAreEqual(true, cells[0, 0].GetStyle().ShrinkToFit, caseName);

            checkShrinkToFit_002(workbook);
            workbook.Save(Constants.destPath + &quot;testShrinkToFit.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testShrinkToFit.xls&quot;);
            checkShrinkToFit_002(workbook);
            workbook.Save(Constants.destPath + &quot;testRotation.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testRotation.xlsx&quot;);
            checkShrinkToFit_002(workbook);
            workbook.Save(Constants.destPath + &quot;testRotation.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testRotation.xml&quot;);
            checkShrinkToFit_002(workbook);
            workbook.Save(Constants.destPath + &quot;testShrinkToFit.xls&quot;);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


