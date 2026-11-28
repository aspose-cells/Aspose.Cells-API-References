---
title: "PivotField.Subtotals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField özelliği. Alanın alt toplamlarını alır veya ayarlar. Yalnızca Satır veya Sütun pivot alanı için"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/subtotals/
---
## PivotField.Subtotals property

Alanının alt toplamlarını alır veya ayarlar. Yalnızca Satır veya Sütun pivot alanı için.

```csharp
public PivotFieldSubtotalType Subtotals { get; set; }
```

### Örnekler

```csharp

[C#]
//Alt toplam yok
rowField.Subtotals = PivotFieldSubtotalType.None;
//Otomatik alt toplamlar
//rowField.Subtotals = PivotFieldSubtotalType.Automatic;
//Tek alt toplam: Sum
//rowField.Subtotals = PivotFieldSubtotalType.Sum;
//Çoklu alt toplamlar: Sum ve count sayıları
//rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

### Ayrıca Bakınız

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


