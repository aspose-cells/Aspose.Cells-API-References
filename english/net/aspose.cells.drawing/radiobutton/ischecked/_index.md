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
// Called: Assert.IsTrue(((RadioButton)workbook.Worksheets[0].Shapes[1]).IsChecked);
[Test]
        public void Property_IsChecked()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET51545.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Type , SheetType.Dialog);
            Assert.IsTrue(((RadioButton)workbook.Worksheets[0].Shapes[1]).IsChecked);
            workbook.Save(Constants.destPath + &quot;CELLSNET51545.xls&quot;);
        }
```

### See Also

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


