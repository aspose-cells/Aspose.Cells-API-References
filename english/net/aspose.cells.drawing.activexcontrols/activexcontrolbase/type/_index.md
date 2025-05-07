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
            var wb = new Workbook(Constants.sourcePath + "CELLSNET53981.xls", loadOptions);
            Shape shape = wb.Worksheets[0].Shapes[0];
            if (shape.ActiveXControl != null)
            {
                if (shape.ActiveXControl.Type == Aspose.Cells.Drawing.ActiveXControls.ControlType.Label)
                {
                    LabelActiveXControl labelActiveX = (LabelActiveXControl)shape.ActiveXControl;
                    if (!string.IsNullOrEmpty(labelActiveX.Caption)
                        && labelActiveX.Caption.Contains("Label_"))
                    {
                        labelActiveX.Caption = labelActiveX.Caption.Replace("Label_", "MyChangedLabel_");
                    }
                }
            }

            wb.Save(Constants.destPath + "CELLSNET53981.xls");
            wb = new Workbook(Constants.destPath + "CELLSNET53981.xls");
            shape = wb.Worksheets[0].Shapes[0];
            LabelActiveXControl labelActiveX0 = (LabelActiveXControl)shape.ActiveXControl;
            Assert.AreEqual("MyChangedLabel_ActiveX",labelActiveX0.Caption);
        }
```

### See Also

* enum [ControlType](../../controltype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


