---
title: ToggleButtonActiveXControl.IsTripleState
second_title: Aspose.Cells for .NET API Reference
description: ToggleButtonActiveXControl property. Indicates how the specified control will display Null values
type: docs
url: /net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/istriplestate/
---
## ToggleButtonActiveXControl.IsTripleState property

Indicates how the specified control will display Null values.

```csharp
public bool IsTripleState { get; set; }
```

### Remarks

| **Setting** | **Description** |
| --- | --- |
| True | The control will cycle through states for Yes, No, and Null values. The control appears dimmed (grayed) when its Value property is set to Null. |
| False | (Default) The control will cycle through states for Yes and No values. Null values display as if they were No values. |

### Examples

```csharp
[C#]
activeXControl.IsTripleState = false;
```

### See Also

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


