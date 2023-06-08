---
title: ShapeCollection.AddActiveXControl
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Creates an Activex Control
type: docs
url: /net/aspose.cells.drawing/shapecollection/addactivexcontrol/
---
## ShapeCollection.AddActiveXControl method

Creates an Activex Control.

```csharp
public Shape AddActiveXControl(ControlType type, int topRow, int top, int leftColumn, int left, 
    int width, int height)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ControlType | The type of the control. |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Shape, in unit of pixel. |
| width | Int32 | Represents the width of Shape, in unit of pixel. |

### Examples

```csharp

[C#]
//add an ActiveX control
Shape activeXControl = shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
```

### See Also

* class [Shape](../../shape/)
* enum [ControlType](../../../aspose.cells.drawing.activexcontrols/controltype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


