---
title: Aspose::Cells::Drawing::ActiveXControls::ToggleButtonActiveXControl::GetValue method
linktitle: GetValue
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ActiveXControls::ToggleButtonActiveXControl::GetValue method. Indicates if the control is checked or not in C++.'
type: docs
weight: 1700
url: /cpp/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/getvalue/
---
## ToggleButtonActiveXControl::GetValue method


Indicates if the control is checked or not.

```cpp
CheckValueType Aspose::Cells::Drawing::ActiveXControls::ToggleButtonActiveXControl::GetValue()
```


## Examples


```cpp
if (activeXControl.GetValue() == CheckValueType::UnChecked)
{
    activeXControl.SetValue(CheckValueType::Checked);
}
```

## See Also

* Enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* Class [ToggleButtonActiveXControl](../)
* Namespace [Aspose::Cells::Drawing::ActiveXControls](../../)
* Library [Aspose.Cells for C++](../../../)
