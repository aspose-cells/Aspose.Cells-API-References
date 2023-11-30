---
title: Aspose::Cells::Drawing::ActiveXControls::ToggleButtonActiveXControl::IsTripleState method
linktitle: IsTripleState
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ActiveXControls::ToggleButtonActiveXControl::IsTripleState method. Indicates how the specified control will display Null values in C++.'
type: docs
weight: 1900
url: /cpp/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/istriplestate/
---
## ToggleButtonActiveXControl::IsTripleState method


Indicates how the specified control will display Null values.

```cpp
bool Aspose::Cells::Drawing::ActiveXControls::ToggleButtonActiveXControl::IsTripleState()
```


<table><tr><th>Setting </th><th>Description  </th></tr><tr><td>True </td><td>The control will cycle through states for Yes, No, and Null values. The control appears dimmed (grayed) when its Value property is set to Null.  </td></tr><tr><td>False </td><td>(Default) The control will cycle through states for Yes and No values. Null values display as if they were No values.  </td></tr></table>

## Examples


```cpp
if (activeXControl.IsTripleState() == true)
{
    activeXControl.SetIsTripleState(false);
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ToggleButtonActiveXControl](../)
* Namespace [Aspose::Cells::Drawing::ActiveXControls](../../)
* Library [Aspose.Cells for C++](../../../)
