---
title: "PivotField.Top10AutoShow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Methode. Konfiguriert die Top10 AutoShow-Einstellungen für dieses Pivot-Feld"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField.Top10AutoShow method

Konfiguriert die Top10-AutoShow-Einstellungen für dieses Pivotfeld.

```csharp
public void Top10AutoShow(bool isAutoShow, bool isTop, int count, int rankBy)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isAutoShow | Boolean | true, um AutoShow zu aktivieren; false, um zu deaktivieren. |
| isTop | Boolean | Wenn true, werden die obersten Elemente angezeigt; false zeigt die untersten Elemente. |
| Anzahl | Int32 | Anzahl der anzuzeigenden oberen/unteren Elemente. |
| rankBy | Int32 | Index des für das Ranking verwendeten Datenfelds. Verwenden Sie -1, um nach den eigenen Werten des Pivot-Elements zu ranken. |

### Hinweise

Diese Methode konfiguriert die [`PivotFieldTop10AutoShowSettings`](../../pivotfieldtop10autoshowsettings/).

XLS-Binärformat: AutoShow (Top10) ist die native und einzige unterstützte Option.

XLSX (OpenXML): Das zugrunde liegende Dateiformat unterstützt Top10 AutoShow, aber die Benutzeroberfläche von Excel 2007 und später stellt dies nur über den Top10-Filter bereit. Wenn XLS-Kompatibilität nicht erforderlich ist, wird empfohlen, stattdessen den Top10-Filter zu verwenden.

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


