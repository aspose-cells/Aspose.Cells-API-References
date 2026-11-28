---
title: "PivotFieldGroupOptions.GroupType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotFieldGroupOptions özelliği. Pivot alanı için grup türünü alır veya ayarlar. Yalnızca tarih saat pivot alanını gruplamak için"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfieldgroupoptions/grouptype/
---
## PivotFieldGroupOptions.GroupType property

Özet alanı için gruplama türünü alır veya ayarlar. Yalnızca tarih saat özet alanı gruplaması için.

```csharp
public PivotGroupByType GroupType { get; set; }
```

### Örnekler

```csharp
//init
PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
// Yılı ve ayı birlikte grupla
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GroupType;
pivotGroupByType = PivotGroupByType.Years | PivotGroupByType.Months;
pivotFieldGroupOptions.GroupType = pivotGroupByType;
```

### Ayrıca Bakınız

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotFieldGroupOptions](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


