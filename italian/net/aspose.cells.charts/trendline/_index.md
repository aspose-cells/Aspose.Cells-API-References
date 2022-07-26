---
title: Trendline
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta una linea di tendenza in un grafico.
type: docs
weight: 980
url: /it/net/aspose.cells.charts/trendline/
---
## Trendline class

Rappresenta una linea di tendenza in un grafico.

```csharp
public class Trendline : Line
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Backward](../../aspose.cells.charts/trendline/backward) { get; set; } | Restituisce o imposta il numero di periodi (o unità su un grafico a dispersione) che la linea di tendenza si estende all'indietro. Il numero di periodi deve essere maggiore o uguale a zero. Se il tipo di grafico è colonna, il numero di periodi deve essere compreso tra 0 e 0,5 |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Specifica la lunghezza della punta della freccia per l'inizio di una riga. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Specifica la larghezza della punta della freccia per l'inizio di una linea. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Specifica una punta di freccia per l'inizio di una riga. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Specifica le maiuscole finali. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Rappresenta ilColor della linea. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Specifica il tipo di linea composta |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Specifica il tipo di linea tratteggiata |
| [DataLabels](../../aspose.cells.charts/trendline/datalabels) { get; } | Rappresenta l'oggetto DataLabels per la serie specificata. |
| [DisplayEquation](../../aspose.cells.charts/trendline/displayequation) { get; set; } | Indica se l'equazione per la linea di tendenza è visualizzata sul grafico (nella stessa etichetta dati del valore R al quadrato). L'impostazione di questa proprietà su True attiva automaticamente le etichette dei dati. |
| [DisplayRSquared](../../aspose.cells.charts/trendline/displayrsquared) { get; set; } | Rappresenta se il valore R al quadrato della linea di tendenza viene visualizzato sul grafico (nella stessa etichetta dati dell'equazione). L'impostazione di questa proprietà su True attiva automaticamente le etichette dei dati. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Specifica la lunghezza della punta della freccia per la fine di una riga. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Specifica la larghezza della punta della freccia per la fine di una riga. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Specifica una freccia per la fine di una riga. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Ottiene o imposta il tipo di formato. |
| [Forward](../../aspose.cells.charts/trendline/forward) { get; set; } | Restituisce o imposta il numero di periodi (o unità su un grafico a dispersione) che la linea di tendenza estende in avanti. Il numero di periodi deve essere maggiore o uguale a zero. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Rappresenta il riempimento sfumato. |
| [Intercept](../../aspose.cells.charts/trendline/intercept) { get; set; } | Restituisce o imposta il punto in cui la linea di tendenza incrocia l'asse dei valori. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Indica se questo stile di linea è assegnato automaticamente. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Indica se il colore della linea è assegnato automaticamente. |
| [IsNameAuto](../../aspose.cells.charts/trendline/isnameauto) { get; set; } | Restituisce se Microsoft Excel determina automaticamente il nome della linea di tendenza. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Indica se la linea è visibile. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Specifica le maiuscole di unione. |
| [LegendEntry](../../aspose.cells.charts/trendline/legendentry) { get; } | Ottiene la voce della legenda in base a questa linea di tendenza |
| [Name](../../aspose.cells.charts/trendline/name) { get; set; } | Restituisce il nome della linea di tendenza. |
| [Order](../../aspose.cells.charts/trendline/order) { get; set; } | Restituisce o imposta l'ordine della linea di tendenza (un numero intero maggiore di 1) quando il tipo di linea di tendenza è Polinomiale. L'ordine deve essere compreso tra 2 e 6. |
| [Period](../../aspose.cells.charts/trendline/period) { get; set; } | Restituisce o imposta il periodo per la linea di tendenza della media mobile. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Rappresenta lo stile della linea. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Ottiene e imposta il colore del tema. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Restituisce o imposta il grado di trasparenza della linea come valore compreso tra 0,0 (opaco) e 1,0 (trasparente). |
| [Type](../../aspose.cells.charts/trendline/type) { get; } | Restituisce il tipo di linea di tendenza. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Ottiene o imposta il[`WeightType`](../../aspose.cells.drawing/weighttype) della linea. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Ottiene o imposta il peso della linea in unità di punti. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Ottiene o imposta lo spessore della linea in unità di pixel. |

### Esempi

```csharp

[C#]

//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();
//Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
int sheetIndex = workbook.Worksheets.Add();
//Ottenere il riferimento del foglio di lavoro appena aggiunto passando il relativo indice del foglio
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Aggiunta di un valore di esempio alla cella "A1".
worksheet.Cells["A1"].PutValue(50);
//Aggiunta di un valore di esempio alla cella "A2".
worksheet.Cells["A2"].PutValue(100);
//Aggiunta di un valore di esempio alla cella "A3".
worksheet.Cells["A3"].PutValue(150);
//Aggiunta di un valore di esempio alla cella "A4".
worksheet.Cells["A4"].PutValue(200);
//Aggiunta di un valore di esempio alla cella "B1".
worksheet.Cells["B1"].PutValue(60);
//Aggiunta di un valore di esempio alla cella "B2".
worksheet.Cells["B2"].PutValue(32);
//Aggiunta di un valore di esempio alla cella "B3".
worksheet.Cells["B3"].PutValue(50);
//Aggiunta di un valore di esempio alla cella "B4".
worksheet.Cells["B4"].PutValue(40);
//Aggiunta di un valore di esempio alla cella "C1" come dati di categoria
worksheet.Cells["C1"].PutValue("Q1");
//Aggiunta di un valore di esempio alla cella "C2" come dati di categoria
worksheet.Cells["C2"].PutValue("Q2");
//Aggiunta di un valore di esempio alla cella "C3" come dati di categoria
worksheet.Cells["C3"].PutValue("Y1");
//Aggiunta di un valore di esempio alla cella "C4" come dati di categoria
worksheet.Cells["C4"].PutValue("Y2");
//Aggiunta di un grafico al foglio di lavoro
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accesso all'istanza del grafico appena aggiunto
Chart chart = worksheet.Charts[chartIndex];
//Aggiunta di NSeries (origine dati grafico) al grafico che va dalla cella "A1" a "B4"
chart.NSeries.Add("A1:B4", true);
//Impostazione dell'origine dati per i dati di categoria di NSeries
chart.NSeries.CategoryData = "C1:C4";
//aggiungendo una linea di tendenza lineare
int index = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[index];
//Impostazione del nome personalizzato della linea di tendenza.
trendline.Name = "Linear";
//Visualizzazione dell'equazione sul grafico
trendline.DisplayEquation = true;
//Visualizzazione del valore R-Squared sul grafico
trendline.DisplayRSquared = true;
//Salvataggio del file Excel
workbook.Save("book1.xls");

[Visual Basic]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()
'Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice del foglio
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Aggiunta di un grafico al foglio di lavoro
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accesso all'istanza del grafico appena aggiunto
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Impostazione dell'origine dati per i dati di categoria di NSeries
Chart.NSeries.CategoryData = "C1:C4"
'aggiungendo una linea di tendenza lineare
Dim index As Int32 = chart.NSeries(0).TrendLines.Add(TrendlineType.Linear)
Dim trendline As Trendline = chart.NSeries(0).TrendLines(index)
'Impostazione del nome personalizzato della linea di tendenza.
trendline.Name = "Linear"
'Visualizzazione dell'equazione sul grafico
trendline.DisplayEquation = True
'Visualizzazione del valore R-quadrato sul grafico
trendline.DisplayRSquared = True
'Salvataggio del file Excel
workbook.Save("book1.xls")
```

### Guarda anche

* class [Line](../../aspose.cells.drawing/line)
* spazio dei nomi [Aspose.Cells.Charts](../../aspose.cells.charts)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
