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
// Called: ((ComboBoxActiveXControl)sheet1.Shapes[0].ActiveXControl).Value = (&amp;quot;a&amp;quot;);
[Test]
        public void Property_Value()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42442.xlsx&quot;);
            Worksheet sheet1 = wb.Worksheets[&quot;Sheet1&quot;];
            ((TextBoxActiveXControl)sheet1.Shapes[1].ActiveXControl).Text = (&quot;def&quot;);
            ((ComboBoxActiveXControl)sheet1.Shapes[0].ActiveXControl).Value = (&quot;a&quot;);
            Assert.AreEqual(&quot;def&quot;, sheet1.Cells[&quot;G10&quot;].StringValue);
            Assert.AreEqual(&quot;a&quot;, sheet1.Cells[&quot;B2&quot;].StringValue);

#if !LINUX_TEST
            //It will cause problem on mono, see:
            //NativeEmfGraphics.SaveImage, CellsHelper.IsBitmapResolutionZero
            sheet1.Shapes.UpdateSelectedValue();
            wb.Save(Constants.destPath +&quot;CELLSJAVA42442.pdf&quot;);
#endif
        }
```

### See Also

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


