---
title: ActiveXControl.Font
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Represents the font of the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/font/
---
## ActiveXControl.Font property

Represents the font of the control.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(19.8,checkBox1.Font.DoubleSize);
[Test]
        public void Property_Font()
        {
            string sourceFolder = path + "CellsJava41225.xlsx";
            Workbook workbook = new Workbook(sourceFolder);
            Shape shape = workbook.Worksheets[0].Shapes[0];
            CheckBoxActiveXControl checkBox1 = (CheckBoxActiveXControl)shape.ActiveXControl;
            Assert.AreEqual("Calibri",checkBox1.Font.Name);
            Assert.AreEqual(19.8,checkBox1.Font.DoubleSize);
        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


