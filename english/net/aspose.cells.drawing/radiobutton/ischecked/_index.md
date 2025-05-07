---
title: RadioButton.IsChecked
second_title: Aspose.Cells for .NET API Reference
description: RadioButton property. Indicates if the radiobutton is checked or not
type: docs
url: /net/aspose.cells.drawing/radiobutton/ischecked/
---
## RadioButton.IsChecked property

Indicates if the radiobutton is checked or not.

```csharp
public bool IsChecked { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(false, shape2.IsChecked);
[Test]
        public void Property_IsChecked()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsJava43474.xls");


            Assert.AreEqual(1, wb.Worksheets[0].Cells["A1"].DoubleValue);




            RadioButton shape1 = (RadioButton)wb.Worksheets[0].Shapes[0];
            RadioButton shape2 = (RadioButton)wb.Worksheets[0].Shapes[1];
            Assert.AreEqual(true, shape1.IsChecked);
            Assert.AreEqual(false, shape2.IsChecked);
            wb.Save(Constants.destPath + "CellsJava434742.xls");

        }
```

### See Also

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


