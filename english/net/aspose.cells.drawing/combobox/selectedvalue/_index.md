---
title: ComboBox.SelectedValue
second_title: Aspose.Cells for .NET API Reference
description: ComboBox property. Gets the selected value of the combox box
type: docs
url: /net/aspose.cells.drawing/combobox/selectedvalue/
---
## ComboBox.SelectedValue property

Gets the selected value of the combox box.

```csharp
public string SelectedValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(comboBox.SelectedValue, "d");
public void ComboBox_Property_SelectedValue()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    ShapeCollection shapes = workbook.Worksheets[0].Shapes;
    for (int i = 0; i < shapes.Count; i++)
    {
        if (shapes[i].MsoDrawingType == MsoDrawingType.ComboBox)
        {
            ComboBox comboBox = (ComboBox)shapes[i];
            Assert.AreEqual(comboBox.SelectedValue, "d");
            break;

        }
    }
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    shapes = workbook.Worksheets[0].Shapes;
    for (int i = 0; i < shapes.Count; i++)
    {
        if (shapes[i].MsoDrawingType == MsoDrawingType.ComboBox)
        {
            ComboBox comboBox = (ComboBox)shapes[i];
            Assert.AreEqual(comboBox.SelectedValue, "d");
            break;
        }
    }
}
```

### See Also

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


