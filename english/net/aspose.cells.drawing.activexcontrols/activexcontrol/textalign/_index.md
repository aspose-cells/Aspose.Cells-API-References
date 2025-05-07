---
title: ActiveXControl.TextAlign
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Represents how to align the text used by the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/textalign/
---
## ActiveXControl.TextAlign property

Represents how to align the text used by the control.

```csharp
public TextAlignmentType TextAlign { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(checkbox.TextAlign, TextAlignmentType.Right);
[Test]
        public void Property_TextAlign()
        {
            Workbook workbook = new Workbook(path + "CELLSJAVA41531.xlsx");
            Shape shape = workbook.Worksheets[0].Shapes[0];
            ActiveXControl checkbox = shape.ActiveXControl;
            Assert.AreEqual(checkbox.TextAlign, TextAlignmentType.Center);
            shape = workbook.Worksheets[0].Shapes[1];
            checkbox = shape.ActiveXControl;
            Assert.AreEqual(checkbox.TextAlign, TextAlignmentType.Right);

        }
```

### See Also

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


