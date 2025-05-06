---
title: Style.RotationAngle
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents text rotation angle
type: docs
url: /net/aspose.cells/style/rotationangle/
---
## Style.RotationAngle property

Represents text rotation angle.

```csharp
public int RotationAngle { get; set; }
```

### Remarks

0: Not rotated.

255: Top to Bottom.

-90: Downward.

90: Upward.

You can set 255 or value ranged from -90 to 90.

### Examples

```csharp
// Called: testAreEqual(styleSrc.RotationAngle, styleDest.RotationAngle, caseName);
private void Property_RotationAngle(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            //compare style.HorizontalAlignment 
            for (int row = 1; row &lt;= 8; row++)
            {
                Style styleSrc = cells[row, 0].GetStyle();
                Style styleDest = cells[row + 16, 0].GetStyle();
                testAreEqual(styleSrc.HorizontalAlignment, styleDest.HorizontalAlignment, caseName);
            }
            //compare style.VerticalAlignment
            for (int row = 1; row &lt;= 5; row++)
            {
                Style styleSrc = cells[row, 2].GetStyle();
                Style styleDest = cells[row + 16, 2].GetStyle();
                testAreEqual(styleSrc.VerticalAlignment, styleDest.VerticalAlignment, caseName);
            }
            //compare style.IsTextWrapped
            testAreEqual(true, cells[1, 4].GetStyle().IsTextWrapped, caseName);
            testAreEqual(true, cells[2, 4].GetStyle().IsTextWrapped, caseName);
            testAreEqual(true, cells[17, 4].GetStyle().IsTextWrapped, caseName);
            testAreEqual(true, cells[18, 4].GetStyle().IsTextWrapped, caseName);
            //compare merged cells
            testAreEqual(true, cells[1, 6].IsMerged, caseName);
            testAreEqual(true, cells[17, 6].IsMerged, caseName);
            //compare Style.TextDirection
            for (int row = 1; row &lt;= 3; row++)
            {
                Style styleSrc = cells[row, 8].GetStyle();
                Style styleDest = cells[row + 16, 8].GetStyle();
                testAreEqual(styleSrc.TextDirection, styleDest.TextDirection, caseName);
            }
            //compare style.rotation
            for (int row = 1; row &lt;= 11; row++)
            {
                Style styleSrc = cells[row, 10].GetStyle();
                Style styleDest = cells[row + 16, 10].GetStyle();
                testAreEqual(styleSrc.RotationAngle, styleDest.RotationAngle, caseName);
            }
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


