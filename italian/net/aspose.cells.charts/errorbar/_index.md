---
title: ErrorBar
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta la barra di errore della serie di dati.
type: docs
weight: 630
url: /it/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Rappresenta la barra di errore della serie di dati.

```csharp
public class ErrorBar : Line
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount) { get; set; } | Rappresenta la quantità di barra di errore.  L'importo deve essere maggiore o uguale a zero. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Specifica la lunghezza della punta della freccia per l'inizio di una riga. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Specifica la larghezza della punta della freccia per l'inizio di una linea. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Specifica una punta di freccia per l'inizio di una riga. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Specifica le maiuscole finali. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Rappresenta ilColor della linea. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Specifica il tipo di linea composta |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Specifica il tipo di linea tratteggiata |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype) { get; set; } | Rappresenta il tipo di visualizzazione della barra di errore. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Specifica la lunghezza della punta della freccia per la fine di una riga. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Specifica la larghezza della punta della freccia per la fine di una riga. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Specifica una freccia per la fine di una riga. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Ottiene o imposta il tipo di formato. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Rappresenta il riempimento sfumato. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indica se questo stile di linea è assegnato automaticamente. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indica se il colore della linea è assegnato automaticamente. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Indica se la linea è visibile. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Specifica le maiuscole di unione. |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue) { get; set; } | Rappresenta la quantità di errore negativa quando il tipo di barra di errore è Personalizzato. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue) { get; set; } | Rappresenta la quantità di errore positiva quando il tipo di barra di errore è Personalizzato. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop) { get; set; } | Indica se la formattazione delle barre di errore con un T-top. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Rappresenta lo stile della linea. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Ottiene e imposta il colore del tema. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Restituisce o imposta il grado di trasparenza della linea come valore compreso tra 0,0 (opaco) e 1,0 (trasparente). |
| [Type](../../aspose.cells.charts/errorbar/type) { get; set; } | Rappresenta il tipo di importo della barra di errore. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Ottiene o imposta il[`WeightType`](../../aspose.cells.drawing/weighttype) della linea. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Ottiene o imposta il peso della linea in unità di punti. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Ottiene o imposta lo spessore della linea in unità di pixel. |

### Esempi

```csharp
[C#]
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["a1"].PutValue(2);
cells["a2"].PutValue(5);
cells["a3"].PutValue(3);
cells["a4"].PutValue(6);
cells["b1"].PutValue(4);
cells["b2"].PutValue(3);
cells["b3"].PutValue(6);
cells["b4"].PutValue(7);

cells["C1"].PutValue("Q1");
cells["C2"].PutValue("Q2");
cells["C3"].PutValue("Y1");
cells["C4"].PutValue("Y2");

int chartIndex = excel.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);

Chart chart = excel.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);

chart.NSeries.CategoryData = "C1:C4";

for(int i = 0; i < chart.NSeries.Count; i ++)
{
	ASeries aseries = chart.NSeries[i];
	aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
	aseries.YErrorBar.Type = ErrorBarType.FixedValue;
	aseries.YErrorBar.Amount = 5;
}

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
Dim cells As Cells =  workbook.Worksheets(0).Cells 
cells("a1").PutValue(2)
cells("a2").PutValue(5)
cells("a3").PutValue(3)
cells("a4").PutValue(6)
cells("b1").PutValue(4)
cells("b2").PutValue(3)
cells("b3").PutValue(6)
cells("b4").PutValue(7)

cells("C1").PutValue("Q1")
cells("C2").PutValue("Q2")
cells("C3").PutValue("Y1")
cells("C4").PutValue("Y2")

Dim chartIndex As Integer =  excel.Worksheets(0).Charts.Add(ChartType.Column,11,0,27,10) 

Dim chart As Chart =  excel.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:B4", True)

chart.NSeries.CategoryData = "C1:C4"

Dim i As Integer
For  i = 0 To chart.NSeries.Count - 1
Dim aseries As ASeries =  chart.NSeries(i) 
aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus
aseries.YErrorBar.Type = ErrorBarType.FixedValue
aseries.YErrorBar.Amount = 5
Next
```

### Guarda anche

* class [Line](../../aspose.cells.drawing/line)
* spazio dei nomi [Aspose.Cells.Charts](../../aspose.cells.charts)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
