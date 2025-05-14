---
title: ListBox.SelectedIndex
second_title: Aspose.Cells for .NET API Reference
description: ListBox property. Gets or sets the index number of the currently selected item in a list box or combo box. Zerobased
type: docs
url: /net/aspose.cells.drawing/listbox/selectedindex/
---
## ListBox.SelectedIndex property

Gets or sets the index number of the currently selected item in a list box or combo box. Zero-based.

```csharp
public int SelectedIndex { get; set; }
```

### Remarks

-1 presents no item is selected.

### Examples

```csharp
// Called: listBox.SelectedIndex = 2;
public void ListBox_Property_SelectedIndex()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Cell cell = workbook.Worksheets[0].Cells["A2"];
    Assert.AreEqual("1", cell.StringValue);
    ListBox listBox = (ListBox)workbook.Worksheets[0].Shapes[3];
    listBox.SelectedIndex = 2;
    Assert.AreEqual("2",cell.StringValue);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


