---
title: ActiveXControlBase.Type
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Gets the type of the ActiveX control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/type/
---
## ActiveXControlBase.Type property

Gets the type of the ActiveX control.

```csharp
public abstract ControlType Type { get; }
```

### Examples

```csharp
// Called: if (shape.ActiveXControl.Type == Aspose.Cells.Drawing.ActiveXControls.ControlType.Label)
[Test]
        public void Property_Type()
        {
            var loadOptions = new LoadOptions
            {
                MemorySetting = MemorySetting.MemoryPreference
            };
            var wb = new Workbook(Constants.sourcePath + &quot;CELLSNET53981.xls&quot;, loadOptions);
            Shape shape = wb.Worksheets[0].Shapes[0];
            if (shape.ActiveXControl != null)
            {
                if (shape.ActiveXControl.Type == Aspose.Cells.Drawing.ActiveXControls.ControlType.Label)
                {
                    LabelActiveXControl labelActiveX = (LabelActiveXControl)shape.ActiveXControl;
                    if (!string.IsNullOrEmpty(labelActiveX.Caption)
                        &amp;&amp; labelActiveX.Caption.Contains(&quot;Label_&quot;))
                    {
                        labelActiveX.Caption = labelActiveX.Caption.Replace(&quot;Label_&quot;, &quot;MyChangedLabel_&quot;);
                    }
                }
            }

            wb.Save(Constants.destPath + &quot;CELLSNET53981.xls&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSNET53981.xls&quot;);
            shape = wb.Worksheets[0].Shapes[0];
            LabelActiveXControl labelActiveX0 = (LabelActiveXControl)shape.ActiveXControl;
            Assert.AreEqual(&quot;MyChangedLabel_ActiveX&quot;,labelActiveX0.Caption);
        }
```

### See Also

* enum [ControlType](../../controltype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


