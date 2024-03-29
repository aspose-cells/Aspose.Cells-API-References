---
title: AddGroupBox
second_title: Aspose.Cells för .NET API-referens
description: Lägger till en GroupBox i kalkylbladet.
type: docs
weight: 110
url: /sv/net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

Lägger till en GroupBox i kalkylbladet.

```csharp
public GroupBox AddGroupBox(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| upperLeftRow | Int32 | Övre vänstra radens index. |
| top | Int32 | Representerar den vertikala förskjutningen av GroupBox från dess vänstra rad, i pixelenhet. |
| upperLeftColumn | Int32 | Övre vänstra kolumnindex. |
| left | Int32 | Representerar den horisontella förskjutningen av GroupBox från dess vänstra kolumn, i pixelenhet. |
| height | Int32 | Representerar höjden på GroupBox, i pixelenhet. |
| width | Int32 | Representerar bredden på GroupBox, i pixelenhet. |

### Returvärde

Ett GroupBox-objekt.

### Exempel

```csharp

[C#]
//lägg till en gruppruta
GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);
```

### Se även

* class [GroupBox](../../groupbox)
* class [ShapeCollection](../../shapecollection)
* namnutrymme [Aspose.Cells.Drawing](../../shapecollection)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
