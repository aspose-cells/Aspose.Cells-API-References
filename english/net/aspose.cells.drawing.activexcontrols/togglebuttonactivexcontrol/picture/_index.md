---
title: ToggleButtonActiveXControl.Picture
second_title: Aspose.Cells for .NET API Reference
description: ToggleButtonActiveXControl property. Gets and sets the data of the picture
type: docs
url: /net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture/
---
## ToggleButtonActiveXControl.Picture property

Gets and sets the data of the picture.

```csharp
public byte[] Picture { get; set; }
```

### Examples

```csharp
[C#]
//e.g byte[] data = File.ReadAllBytes("image.png");
byte[] data = null;
if(activeXControl.Picture != null)
{
    activeXControl.Picture = data;
}
```

### See Also

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


