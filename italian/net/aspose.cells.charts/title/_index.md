---
title: Title
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula loggetto che rappresenta il titolo del grafico o dellasse.
type: docs
weight: 970
url: /it/net/aspose.cells.charts/title/
---
## Title class

Incapsula l'oggetto che rappresenta il titolo del grafico o dell'asse.

```csharp
public class Title : ChartTextFrame
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Ottiene il[`la zona`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | Vero se il testo nell'oggetto cambia la dimensione del carattere quando cambia la dimensione dell'oggetto. Il valore predefinito è Vero. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Ottiene e imposta la modalità di visualizzazione dello sfondo |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Ottiene il[`confine`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Rappresenta l'altezza della posizione predefinita |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Rappresenta la larghezza della posizione predefinita |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Rappresenta x della posizione predefinita |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Rappresenta y della posizione predefinita |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Ottiene e imposta la direzione del testo. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | Ottiene a[`Font`](../chartframe/font) oggetto dell'oggetto ChartFrame specificato. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Ottiene o imposta l'altezza del frame in unità di 1/4000 dell'area del grafico. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indica se la cornice del grafico è dimensionata automaticamente. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Indica che il testo è stato generato automaticamente. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indica se queste etichette dati sono state eliminate. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indica se la dimensione dell'area del tracciato include i segni di graduazione e le etichette degli assi. False specifica che la dimensione determina la dimensione dell'area del tracciato, i segni di graduazione e le etichette degli assi. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Ottiene o imposta se una forma deve essere adattata automaticamente per contenere completamente il testo descritto al suo interno. L'adattamento automatico è quando il testo all'interno di una forma viene ridimensionato in modo da contenere tutto il testo all'interno. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Ottiene o imposta un valore che indica se il testo è a capo. |
| [IsVisible](../../aspose.cells.charts/title/isvisible) { get; set; } | Indica se il titolo è visibile. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Ottiene e imposta un riferimento al foglio di lavoro. |
| [OverLay](../../aspose.cells.charts/title/overlay) { get; set; } | Rappresenta il titolo centrato in sovrapposizione sul grafico senza ridimensionare il grafico. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Rappresenta l'ordine di lettura del testo. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Rappresenta l'angolo di rotazione del testo. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Vero se la cornice ha un'ombra. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Ottiene il[`ShapeProperties`](../chartframe/shapeproperties) oggetto. |
| override [Text](../../aspose.cells.charts/title/text) { get; set; } | Ottiene o imposta il testo dell'etichetta dell'unità di visualizzazione. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Ottiene e imposta l'allineamento orizzontale del testo. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Ottiene o imposta l'allineamento verticale del testo del testo. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Ottiene o imposta la larghezza del fotogramma in unità di 1/4000 dell'area del grafico. |
| override [X](../../aspose.cells.charts/title/x) { get; set; } | Ottiene o imposta la coordinata x dell'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| override [Y](../../aspose.cells.charts/title/y) { get; set; } | Ottiene o imposta la coordinata y dell'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Characters](../../aspose.cells.charts/title/characters#characters_1)() | Ottiene la formattazione RTF di questo titolo. |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Restituisce un oggetto Caratteri che rappresenta un intervallo di caratteri all'interno del testo. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Imposta la posizione del frame su automatic |

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
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];

//Impostazione del titolo di un grafico
chart.Title.Text = "Title";
//Impostazione del colore del carattere del titolo del grafico su blu
chart.Title.Font.Color = Color.Blue;
//Impostazione del titolo dell'asse di categoria del grafico
chart.CategoryAxis.Title.Text = "Category";
//Impostazione del titolo dell'asse dei valori del grafico
chart.ValueAxis.Title.Text = "Value";

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

'Impostazione del titolo di un grafico
chart.Title.Text = "Title"
'Impostare il colore del carattere del titolo del grafico su blu
chart.Title.Font.Color = Color.Blue
'Impostazione del titolo dell'asse di categoria del grafico
chart.CategoryAxis.Title.Text = "Category"
'Impostazione del titolo dell'asse dei valori del grafico
chart.ValueAxis.Title.Text = "Value"

```

### Guarda anche

* class [ChartTextFrame](../charttextframe)
* spazio dei nomi [Aspose.Cells.Charts](../../aspose.cells.charts)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
