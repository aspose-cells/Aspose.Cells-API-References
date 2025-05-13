---
title: ComboBox.SelectedIndex
second_title: Aspose.Cells for .NET API Reference
description: ComboBox property. Gets or sets the index number of the currently selected item in a list box or combo box. Zerobased
type: docs
url: /net/aspose.cells.drawing/combobox/selectedindex/
---
## ComboBox.SelectedIndex property

Gets or sets the index number of the currently selected item in a list box or combo box. Zero-based.

```csharp
public int SelectedIndex { get; set; }
```

### Remarks

-1 presents no item is selected.

### Examples

```csharp
// Called: Assert.AreEqual(box.SelectedIndex, 4);
public void ComboBox_Property_SelectedIndex()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "ComboBoxCopyTest.xlsx");
    Workbook dest = new Workbook();
    dest.Copy(workbook);
     ComboBox box = null;
     Worksheet worksheet = dest.Worksheets[0];
    foreach (Shape shape in worksheet.Shapes)
    {
        box = shape as ComboBox;
        if (box != null) break;
    }
    if (box != null)
    {
        Assert.AreEqual(box.SelectedIndex, 4);
    }
}
```

### See Also

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


