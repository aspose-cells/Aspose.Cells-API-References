---
title: SetLinkedCell
second_title: Aspose.Cells for .NET API Reference
description: Sets the range linked to the controls value.
type: docs
weight: 1180
url: /net/aspose.cells.drawing/shape/setlinkedcell/
---
## Shape.SetLinkedCell method

Sets the range linked to the control's value.

```csharp
public void SetLinkedCell(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The range linked to the control's value. |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |

### Examples

```csharp

[C#]
//After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.

//ActiveX Controls
//Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);

//Form Controls
Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddScrollBar(2, 0, 2, 0, 130, 30);

//Sets the range linked to the control's value.
scrollBar.SetLinkedCell("$A$12", false, true);

```

### See Also

* class [Shape](../../shape)
* namespace [Aspose.Cells.Drawing](../../shape)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
