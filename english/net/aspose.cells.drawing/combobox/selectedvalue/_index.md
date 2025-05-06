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
// Called: Assert.AreEqual(((ComboBox)shapes[7]).SelectedValue, &amp;quot;Supplemental&amp;quot;);
[Test]
        public void Property_SelectedValue()
        {
            //Supplemental
            
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Defect+153972+-+Macros+and+Dropdowns.xlsm&quot;);
            ShapeCollection shapes = workbook.Worksheets[&quot;Supplemental Non-Stat Sample-1&quot;].Shapes;
            Assert.AreEqual(((ComboBox)shapes[7]).SelectedValue, &quot;Supplemental&quot;);
        }
```

### See Also

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


