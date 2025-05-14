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
// Called: ((RadioButton)wb.Worksheets["sheet4"].Shapes[1]).IsChecked = true;
public void RadioButton_Property_IsChecked()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    ((RadioButton)wb.Worksheets["sheet4"].Shapes[1]).IsChecked = true;
    Assert.AreEqual("2",wb.Worksheets["sheet4"].Cells["K7"].StringValue);
    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


