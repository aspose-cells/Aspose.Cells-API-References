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
// Called: Assert.AreEqual(wb.Worksheets[0].Cells["B2"].GetStyle().RotationAngle, 90);
[Test]
        public void Property_RotationAngle()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45170/";
            Workbook wb = new Workbook(filePath + "sample.xlsx");
            wb.Save(CreateFolder(filePath) + "out.html");

            wb = new Workbook(filePath + "sample.xlsx");
            wb.Worksheets[0].AutoFitColumns();
            wb.Save(CreateFolder(filePath) + "out_autofit.html");
            Assert.AreEqual(wb.Worksheets[0].Cells["B1"].GetStyle().RotationAngle, 0);
            Assert.AreEqual(wb.Worksheets[0].Cells["B2"].GetStyle().RotationAngle, 90);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


