---
title: Line
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula loggetto che rappresenta il formato della linea.
type: docs
weight: 2200
url: /it/net/aspose.cells.drawing/line/
---
## Line class

Incapsula l'oggetto che rappresenta il formato della linea.

```csharp
public class Line
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Specifica la lunghezza della punta della freccia per l'inizio di una riga. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Specifica la larghezza della punta della freccia per l'inizio di una linea. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Specifica una punta di freccia per l'inizio di una riga. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Specifica le maiuscole finali. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Rappresenta ilColor della linea. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Specifica il tipo di linea composta |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Specifica il tipo di linea tratteggiata |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Specifica la lunghezza della punta della freccia per la fine di una riga. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Specifica la larghezza della punta della freccia per la fine di una riga. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Specifica una freccia per la fine di una riga. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Ottiene o imposta il tipo di formato. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Rappresenta il riempimento sfumato. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indica se questo stile di linea è assegnato automaticamente. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indica se il colore della linea è assegnato automaticamente. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Indica se la linea è visibile. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Specifica le maiuscole di unione. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Rappresenta lo stile della linea. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Ottiene e imposta il colore del tema. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Restituisce o imposta il grado di trasparenza della linea come valore compreso tra 0,0 (opaco) e 1,0 (trasparente). |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Ottiene o imposta il[`WeightType`](../weighttype) della linea. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Ottiene o imposta il peso della linea in unità di punti. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Ottiene o imposta lo spessore della linea in unità di pixel. |

### Esempi

```csharp

[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);

int chartIndex = sheet.Charts.Add(ChartType.Line, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
//Applicazione di uno stile di linea tratteggiata sulle linee di un NSeries
chart.NSeries[0].Border.Style = LineType.Dot;
chart.NSeries[0].Border.Color = Color.Red;
//Applicazione di uno stile di marcatore triangolare sui marcatori di dati di un NSeries
chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
//Impostazione del peso di tutte le righe in un NSeries su medio
chart.NSeries[0].Border.Weight = WeightType.MediumLine;

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)    ///
Dim chart as Chart = sheet.Charts(chartIndex)
'Applicazione di uno stile di linea tratteggiata sulle linee di un NSeries
chart.NSeries(0).Border.Style = LineType.Dot
chart.NSeries(0).Border.Color = Color.Red
'Applicazione di uno stile di marcatore triangolare sui marcatori di dati di un NSeries
chart.NSeries(0).Marker.MarkerStyle = ChartMarkerType.Triangle
'Impostazione del peso di tutte le linee in un NSeries su medio
chart.NSeries(0).Border.Weight = WeightType.MediumLine
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
