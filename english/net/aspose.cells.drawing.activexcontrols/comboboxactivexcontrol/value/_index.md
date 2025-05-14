---
title: ComboBoxActiveXControl.Value
second_title: Aspose.Cells for .NET API Reference
description: ComboBoxActiveXControl property. Gets and sets the value of the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/value/
---
## ComboBoxActiveXControl.Value property

Gets and sets the value of the control.

```csharp
public string Value { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("a",((Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl).Value);
public void ComboBoxActiveXControl_Property_Value()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet sheet1 = wb.Worksheets["sheet1"];
    Shape shape = sheet1.Shapes[0];
    sheet1.Cells["B2"].PutValue("a");
    sheet1.Shapes.UpdateSelectedValue();
   Assert.AreEqual("a",((Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl).Value);
}
```

### See Also

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


