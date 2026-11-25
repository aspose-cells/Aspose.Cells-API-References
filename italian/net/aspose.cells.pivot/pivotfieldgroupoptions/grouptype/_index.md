---
title: "PivotFieldGroupOptions.GroupType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFieldGroupOptions. Ottiene o imposta il tipo di raggruppamento per il campo pivot. Solo per il raggruppamento di campi pivot data/ora"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldgroupoptions/grouptype/
---
## PivotFieldGroupOptions.GroupType property

Ottiene o imposta il tipo di raggruppamento per il campo pivot. Solo per il raggruppamento del campo pivot data e ora.

```csharp
public PivotGroupByType GroupType { get; set; }
```

### Esempi

```csharp
//init
PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
// Raggruppa per anno e mese insieme
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GroupType;
pivotGroupByType = PivotGroupByType.Years | PivotGroupByType.Months;
pivotFieldGroupOptions.GroupType = pivotGroupByType;
```

### Vedi anche

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotFieldGroupOptions](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


