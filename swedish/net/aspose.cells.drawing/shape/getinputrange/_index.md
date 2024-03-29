---
title: GetInputRange
second_title: Aspose.Cells för .NET API-referens
description: Får intervallet som används för att fylla kontrollen.
type: docs
weight: 1040
url: /sv/net/aspose.cells.drawing/shape/getinputrange/
---
## Shape.GetInputRange method

Får intervallet som används för att fylla kontrollen.

```csharp
public string GetInputRange(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Huruvida formeln behöver formateras efter språk. |

### Returvärde

Området som används för att fylla kontrollen.

### Exempel

```csharp

[C#]
string range = shape.GetInputRange(false, true);
//Om det lyckas kommer ett värde som "$A$1:$A$3" att returneras
```

### Se även

* class [Shape](../../shape)
* namnutrymme [Aspose.Cells.Drawing](../../shape)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
