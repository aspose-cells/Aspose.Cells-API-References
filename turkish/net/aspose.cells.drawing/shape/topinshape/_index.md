---
title: "Shape.TopInShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape özelliği. Şeklin, üst ebeveyn şeklinin üst kenarından, ebeveyn şeklin yüksekliğinin 1/4000 birimi cinsinden dikey offsetini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing/shape/topinshape/
---
## Shape.TopInShape property

Şeklin üst kenarından ebeveyn şeklin üst kenarına olan dikey offsetini, ebeveyn şeklin yüksekliğinin 1/4000 birimi cinsinden temsil eder.

```csharp
public int TopInShape { get; set; }
```

### Açıklamalar

Yalnızca bu şekil grup veya grafik içinde olduğunda uygulanır.

### Örnekler

```csharp

[C#]
if (shape.IsInGroup && shape.TopInShape == 8000)
    shape.TopInShape = 4000;
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


