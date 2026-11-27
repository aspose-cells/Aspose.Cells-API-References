---
title: "PivotField.Top10AutoShow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Konfigurerar Top10 AutoShow-inställningar för detta pivotfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/top10autoshow/
---
## PivotField.Top10AutoShow method

Konfigurerar Top10 AutoShow-inställningar för detta pivottfält.

```csharp
public void Top10AutoShow(bool isAutoShow, bool isTop, int count, int rankBy)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAutoShow | Boolean | true för att aktivera AutoShow; false för att inaktivera. |
| isTop | Boolean | Om true visas toppobjekten; false visas bottenobjekten. |
| antal | Int32 | Antal topp-/bottenobjekt att visa. |
| rankBy | Int32 | Index för datafält som används för rangordning. Använd -1 för att rangordna efter pivot item's egna värden. |

### Anmärkningar

Denna metod konfigurerar [`PivotFieldTop10AutoShowSettings`](../../pivotfieldtop10autoshowsettings/).

XLS binärt format: AutoShow (Top10) är det inbyggda och enda stödda alternativet.

XLSX (OpenXML): Det underliggande filformatet stöder Top10 AutoShow, men Excel 2007 och senare användargränssnitt visar detta endast via Top10-filter. Om XLS-kompatibilitet inte krävs rekommenderas att använda Top10-filter istället.

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


