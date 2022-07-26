---
title: ChartArea
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula loggetto che rappresenta larea del grafico nel foglio di lavoro.
type: docs
weight: 440
url: /it/net/aspose.cells.charts/chartarea/
---
## ChartArea class

Incapsula l'oggetto che rappresenta l'area del grafico nel foglio di lavoro.

```csharp
public class ChartArea : ChartFrame
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
| override [Font](../../aspose.cells.charts/chartarea/font) { get; } | Ottiene a[`Font`](./font) oggetto dell'oggetto chartarea specificato. |
| override [Height](../../aspose.cells.charts/chartarea/height) { get; set; } | Ottiene o imposta l'offset verticale dalla riga dell'angolo inferiore destro. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indica se la cornice del grafico è dimensionata automaticamente. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indica se la dimensione dell'area del tracciato include i segni di graduazione e le etichette degli assi. False specifica che la dimensione determina la dimensione dell'area del tracciato, i segni di graduazione e le etichette degli assi. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Vero se la cornice ha un'ombra. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Ottiene il[`ShapeProperties`](../chartframe/shapeproperties) oggetto. |
| override [Width](../../aspose.cells.charts/chartarea/width) { get; set; } | Ottiene o imposta l'offset orizzontale dalla relativa colonna nell'angolo inferiore destro. |
| override [X](../../aspose.cells.charts/chartarea/x) { get; set; } | Ottiene o ottiene l'offset orizzontale dalla colonna dell'angolo superiore sinistro. |
| override [Y](../../aspose.cells.charts/chartarea/y) { get; set; } | Ottiene o ottiene l'offset verticale dalla riga dell'angolo superiore sinistro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Imposta la posizione del frame su automatic |

### Esempi

```csharp

[C#]

//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();

//Ottenere il riferimento del primo foglio di lavoro
Worksheet worksheet = workbook.Worksheets[0];

//Aggiunta di un valore di esempio alla cella "A1".
worksheet.Cells["A1"].PutValue(50);

//Aggiunta di un valore di esempio alla cella "A2".
worksheet.Cells["A2"].PutValue(100);

//Aggiunta di un valore di esempio alla cella "A3".
worksheet.Cells["A3"].PutValue(150);

//Aggiunta di un valore di esempio alla cella "B1".
worksheet.Cells["B1"].PutValue(60);

//Aggiunta di un valore di esempio alla cella "B2".
worksheet.Cells["B2"].PutValue(32);

//Aggiunta di un valore di esempio alla cella "B3".
worksheet.Cells["B3"].PutValue(50);

//Aggiunta di un grafico al foglio di lavoro
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

//Accesso all'istanza del grafico appena aggiunto
Chart chart = worksheet.Charts[chartIndex];

//Aggiunta di NSeries (origine dati grafico) al grafico che va dalla cella "A1" a "B3"
chart.NSeries.Add("A1:B3", true);

//Come ottenere l'area del grafico
ChartArea chartArea = chart.ChartArea;

//Impostazione del colore di primo piano dell'area del grafico
chartArea.Area.ForegroundColor = Color.Yellow;

//Impostazione dell'ombra dell'area del grafico
chartArea.Shadow = true;

//Salvataggio del file Excel
workbook.Save("book1.xls");

[VB.NET]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()

'Ottenere il riferimento del primo foglio di lavoro
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)

'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)

'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)

'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)

'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)

'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)

'Aggiunta di un grafico al foglio di lavoro
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)

'Accesso all'istanza del grafico appena aggiunto
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

'Ottenere l'area del grafico
Dim chartArea As ChartArea = chart.ChartArea

'Impostazione del colore di primo piano dell'area del grafico
chartArea.Area.ForegroundColor = Color.Yellow

'Impostazione dell'ombra dell'area del grafico
chartArea.Shadow = True

'Salvataggio del file Excel
workbook.Save("book1.xls")
```

### Guarda anche

* class [ChartFrame](../chartframe)
* spazio dei nomi [Aspose.Cells.Charts](../../aspose.cells.charts)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
