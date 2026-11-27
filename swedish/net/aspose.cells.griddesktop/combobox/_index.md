---
title: "Klass ComboBox"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridDesktop.ComboBox klass. Representerar en cell‑combobox‑kontroll"
type: docs
url: /sv/net/aspose.cells.griddesktop/combobox/
---
## ComboBox class

Representerar en cellkombinationsruta‑kontroll.

```csharp
public class ComboBox : CellControl
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Height](../../aspose.cells.griddesktop/combobox/height/) { get; set; } | Hämtar eller anger höjden på listkontrollen. |
| [IsInputable](../../aspose.cells.griddesktop/combobox/isinputable/) { get; set; } | Anger om användaren kan mata in text i comboboxen. Den inmatade texten sparas som cellens värde. Standardvärdet är "false". |
| [Items](../../aspose.cells.griddesktop/combobox/items/) { get; } | Hämtar ett objekt som representerar samlingen av objekt som finns i denna ComboBox. |
| [SelectedIndex](../../aspose.cells.griddesktop/combobox/selectedindex/) { get; set; } | Hämtar eller anger indexet som specificerar det för närvarande valda objektet. Att ange indexet kommer automatiskt att anropa metoden GridDesktop.RunAllFormulas om egenskapen GridDesktop.RecalculateFormulas är sann. |
| [Text](../../aspose.cells.griddesktop/cellcontrol/text/) { get; set; } | Hämtar eller anger texten som är associerad med den här kontrollen.(Ärvd från [`CellControl`](../cellcontrol/).) |
| [Values](../../aspose.cells.griddesktop/combobox/values/) { get; } | Hämtar ett objekt som representerar samlingen av värden som finns i denna ComboBox. |
| [Width](../../aspose.cells.griddesktop/combobox/width/) { get; set; } | Hämtar eller anger bredden på listkontrollen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetSelectedIndex](../../aspose.cells.griddesktop/combobox/setselectedindex/)(int) | Anger det valda indexet för ComboBoxen. Detta beräknar inte formeln. För att beräkna formeln måste GridDesktop.RunAllFormulas anropas manuellt. Det kommer inte att automatiskt beräkna formler i något fall, även om GridDesktop.RecalculateFormulas är sann. |

### Se även

* class [CellControl](../cellcontrol/)
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


