---
title: ListBox.IsSelected
second_title: Aspose.Cells for .NET API Reference
description: ListBox method. Indicates whether the item is selected
type: docs
url: /net/aspose.cells.drawing/listbox/isselected/
---
## ListBox.IsSelected method

Indicates whether the item is selected.

```csharp
public bool IsSelected(int itemIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| itemIndex | Int32 | The item index. |

### Return Value

whether the item is selected.

### Examples

```csharp
// Called: Assert.AreEqual(comboBox.IsSelected(1), false);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ListBoxIssue.xlsx");
            ListBox comboBox = (ListBox)workbook.Worksheets[0].Shapes[0];
            Assert.AreEqual(comboBox.IsSelected(0), false);
            Assert.AreEqual(comboBox.IsSelected(1), false);
            Assert.AreEqual(comboBox.IsSelected(2), false);
        }
```

### See Also

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


