---
title: AddIdentify
second_title: Aspose.Cells für .NET-API-Referenz
description: Legt fest welche Elementbezeichnung in jedem Seitenfeld verwendet werden soll um den Datenbereich zu identifizieren. Die pageItemIndex.Length muss gleich PageFieldCount sein also fügen Sie bitte zuerst das Seitenfeld hinzu.
type: docs
weight: 30
url: /de/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

Legt fest, welche Elementbezeichnung in jedem Seitenfeld verwendet werden soll, um den Datenbereich zu identifizieren. Die pageItemIndex.Length muss gleich PageFieldCount sein, also fügen Sie bitte zuerst das Seitenfeld hinzu.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rangeIndex | Int32 | Der Konsolidierungsdatenbereichsindex. |
| pageItemIndex | Int32[] | Der Seitenelementindex in jedem Seitenfeld. pageItemIndex[2] = 1 bedeutet, dass das zweite Element im dritten Feld verwendet wird, um diesen Bereich zu identifizieren. pageItemIndex[1] = -1 bedeutet, dass kein Element im zweiten Feld verwendet werden soll Identifizieren Sie diesen Bereich und MS erstellt automatisch ein "leeres" Element im zweiten Feld, um diesen Bereich zu identifizieren. |

### Siehe auch

* class [PivotPageFields](../../pivotpagefields)
* namensraum [Aspose.Cells.Pivot](../../pivotpagefields)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
