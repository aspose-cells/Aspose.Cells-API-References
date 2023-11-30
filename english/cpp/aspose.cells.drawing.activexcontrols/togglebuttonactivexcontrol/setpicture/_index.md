﻿---
title: Aspose::Cells::Drawing::ActiveXControls::ToggleButtonActiveXControl::SetPicture method
linktitle: SetPicture
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ActiveXControls::ToggleButtonActiveXControl::SetPicture method. Gets and sets the data of the picture in C++.'
type: docs
weight: 1400
url: /cpp/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/setpicture/
---
## ToggleButtonActiveXControl::SetPicture method


Gets and sets the data of the picture.

```cpp
void Aspose::Cells::Drawing::ActiveXControls::ToggleButtonActiveXControl::SetPicture(const Vector<uint8_t> &value)
```


## Examples


```cpp
Vector<uint8_t> data{ 0 };//Read an image to 'data'.e.g "image.png"(Note: You need to read the data into this variable.)
if (!activeXControl.GetPicture().IsNull())
{
    activeXControl.SetPicture(data);
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ToggleButtonActiveXControl](../)
* Namespace [Aspose::Cells::Drawing::ActiveXControls](../../)
* Library [Aspose.Cells for C++](../../../)
