---
title: DisplayUnitLabel
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta letichetta dellunità di visualizzazione.
type: docs
weight: 600
url: /it/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

Rappresenta l'etichetta dell'unità di visualizzazione.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Ottiene il[`la zona`](../chartframe/area) . |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont) { get; set; } | Vero se il testo nell'oggetto cambia la dimensione del carattere quando cambia la dimensione dell'oggetto. Il valore predefinito è Vero. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Ottiene e imposta la modalità di visualizzazione dello sfondo |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Ottiene il[`confine`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Rappresenta l'altezza della posizione predefinita |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Rappresenta la larghezza della posizione predefinita |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Rappresenta x della posizione predefinita |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Rappresenta y della posizione predefinita |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Ottiene e imposta la direzione del testo. |
| override [Font](../../aspose.cells.charts/displayunitlabel/font) { get; } | Ottiene a[`Font`](./font) oggetto dell'oggetto ChartFrame specificato. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Ottiene o imposta l'altezza del frame in unità di 1/4000 dell'area del grafico. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indica se la cornice del grafico è dimensionata automaticamente. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Indica che il testo è stato generato automaticamente. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indica se queste etichette dati sono state eliminate. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indica se la dimensione dell'area del tracciato include i segni di graduazione e le etichette degli assi. False specifica che la dimensione determina la dimensione dell'area del tracciato, i segni di graduazione e le etichette degli assi. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Ottiene o imposta se una forma deve essere adattata automaticamente per contenere completamente il testo descritto al suo interno. L'adattamento automatico è quando il testo all'interno di una forma viene ridimensionato in modo da contenere tutto il testo all'interno. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Ottiene o imposta un valore che indica se il testo è a capo. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Ottiene e imposta un riferimento al foglio di lavoro. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Rappresenta l'ordine di lettura del testo. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Rappresenta l'angolo di rotazione del testo. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Vero se la cornice ha un'ombra. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Ottiene il[`ShapeProperties`](../chartframe/shapeproperties) oggetto. |
| override [Text](../../aspose.cells.charts/displayunitlabel/text) { get; set; } | Ottiene o imposta il testo dell'etichetta dell'unità di visualizzazione. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Ottiene e imposta l'allineamento orizzontale del testo. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Ottiene o imposta l'allineamento verticale del testo del testo. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Ottiene o imposta la larghezza del fotogramma in unità di 1/4000 dell'area del grafico. |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Ottiene o imposta la coordinata x dell'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Ottiene o imposta la coordinata y dell'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Restituisce un oggetto Caratteri che rappresenta un intervallo di caratteri all'interno del testo. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Imposta la posizione del frame su automatic |

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
//Impostazione dell'unità di visualizzazione dell'asse del valore(Y).
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
//Impostazione dell'etichetta personalizzata dell'unità di visualizzazione
displayUnitLabel.Text = "100";
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
'Impostazione dell'unità di visualizzazione dell'asse del valore (Y).
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds
Dim displayUnitLabel As DisplayUnitLabel = chart.ValueAxis.DisplayUnitLabel
'Impostazione dell'etichetta personalizzata dell'unità di visualizzazione
displayUnitLabel.Text = "100"
'Salvataggio del file Excel
workbook.Save("book1.xls")
```

### Guarda anche

* class [ChartTextFrame](../charttextframe)
* spazio dei nomi [Aspose.Cells.Charts](../../aspose.cells.charts)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
