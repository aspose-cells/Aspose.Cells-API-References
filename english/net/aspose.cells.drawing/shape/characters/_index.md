---
title: Shape.Characters
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Returns a Characters object that represents a range of characters within the text
type: docs
url: /net/aspose.cells.drawing/shape/characters/
---
## Shape.Characters method

Returns a Characters object that represents a range of characters within the text.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The index of the start of the character. |
| length | Int32 | The number of characters. |

### Return Value

Characters object.

### Remarks

This method only works on shape with title.

### Examples

```csharp

[C#]
Aspose.Cells.FontSetting fontSetting = shape.Characters(0, 4);
```

### See Also

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


