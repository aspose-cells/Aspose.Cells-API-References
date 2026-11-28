---
title: "Shape.LeftInShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin, üst şeklin sol kenarından yatay ofsetini, üst şeklin genişliğinin 1/4000'i biriminde temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/shape/leftinshape/
---
## Shape.LeftInShape property

Şeklin, sol ana şeklin sol kenarından yatay ofsetini, ana şeklin genişliğinin 1/4000 birimi olarak temsil eder.

```csharp
public int LeftInShape { get; set; }
```

### Açıklamalar

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

### Örnekler

```csharp

[C#]
if (shape.IsInGroup && shape.LeftInShape == 2000)
    shape.LeftInShape = 4000;
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


