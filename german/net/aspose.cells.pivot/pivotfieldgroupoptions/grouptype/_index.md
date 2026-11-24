---
title: "PivotFieldGroupOptions.GroupType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotFieldGroupOptions Eigenschaft. Ruft den Gruppierungstyp für das Pivot-Feld ab oder legt ihn fest. Nur für die Gruppierung von Datum‑Uhrzeit-Pivot‑Feldern"
type: docs
url: /de/net/aspose.cells.pivot/pivotfieldgroupoptions/grouptype/
---
## PivotFieldGroupOptions.GroupType property

Liest oder setzt den Gruppierungstyp für das Pivot‑Feld. Nur für die Gruppierung von Datum‑Uhrzeit‑Pivot‑Feldern.

```csharp
public PivotGroupByType GroupType { get; set; }
```

### Beispiele

```csharp
//init
PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
// Nach Jahr und Monat zusammen gruppieren
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GroupType;
pivotGroupByType = PivotGroupByType.Years | PivotGroupByType.Months;
pivotFieldGroupOptions.GroupType = pivotGroupByType;
```

### Siehe auch

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotFieldGroupOptions](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


