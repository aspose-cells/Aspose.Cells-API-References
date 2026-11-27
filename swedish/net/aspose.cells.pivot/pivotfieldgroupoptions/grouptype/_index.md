---
title: "PivotFieldGroupOptions.GroupType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFieldGroupOptions egenskap. Hämtar eller anger grupperingstypen för pivottfältet. Endast för gruppering av datum‑tid-pivottfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldgroupoptions/grouptype/
---
## PivotFieldGroupOptions.GroupType property

Hämtar eller anger grupperingstypen för pivottfält. Endast för gruppering av datum‑tid‑pivottfält.

```csharp
public PivotGroupByType GroupType { get; set; }
```

### Exempel

```csharp
//init
PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
// Gruppera efter år och månad tillsammans
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GroupType;
pivotGroupByType = PivotGroupByType.Years | PivotGroupByType.Months;
pivotFieldGroupOptions.GroupType = pivotGroupByType;
```

### Se även

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotFieldGroupOptions](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


