---
title: Aspose::Cells::Drawing::Shape::GetActiveXControl method
linktitle: GetActiveXControl
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::GetActiveXControl method. Gets the ActiveX control in C++.'
type: docs
weight: 17800
url: /cpp/aspose.cells.drawing/shape/getactivexcontrol/
---
## Shape::GetActiveXControl method


Gets the ActiveX control.

```cpp
ActiveXControl Aspose::Cells::Drawing::Shape::GetActiveXControl()
```


## Examples


```cpp
if(!shape.GetActiveXControl().IsNull())
{
    CheckBoxActiveXControl checkBox1 = (CheckBoxActiveXControl)shape.GetActiveXControl();
    //The font name of CheckBox
    U16String fontName = checkBox1.GetFont().GetName();
}
```

## See Also

* Class [ActiveXControl](../../../aspose.cells.drawing.activexcontrols/activexcontrol/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
