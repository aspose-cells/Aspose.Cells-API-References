---
title: FillFormat
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula loggetto che rappresenta la formattazione di riempimento per una forma.
type: docs
weight: 1970
url: /it/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Incapsula l'oggetto che rappresenta la formattazione di riempimento per una forma.

```csharp
public class FillFormat
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Ottiene e imposta il tipo di riempimento |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Restituisce il colore della sfumatura 1 per il riempimento specificato. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Restituisce il colore della sfumatura 2 per il riempimento specificato. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Restituisce il tipo di colore sfumato per il riempimento specificato. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Restituisce il grado di sfumatura per il riempimento specificato. Vale solo per Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Ottiene[`GradientFill`](./gradientfill) oggetto. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Restituisce lo stile del gradiente per il riempimento specificato. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Restituisce la variante del gradiente per il riempimento specificato. Vale solo per Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Ottiene e imposta i dati dell'immagine dell'immagine. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Rappresenta il modello di visualizzazione di un'area. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Ottiene[`PatternFill`](./patternfill) oggetto. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Ottiene e imposta il tipo di formato immagine. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Restituisce il colore predefinito del gradiente per il riempimento specificato. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Ottiene e imposta la scala del formato dell'immagine. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Ottiene[`SolidFill`](./solidfill) oggetto. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Rappresenta il tipo di trama per il riempimento specificato. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Ottiene[`TextureFill`](./texturefill) oggetto. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Restituisce o imposta il grado di trasparenza dell'area come un valore compreso tra 0,0 (opaco) e 1,0 (trasparente). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode)() | Ottiene il codice hash. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Imposta il riempimento specificato su una sfumatura di un colore. Si applica solo a Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Imposta il riempimento specificato su una sfumatura di colore preimpostata. Si applica solo a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Imposta il riempimento specificato su una sfumatura a due colori. Si applica solo a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Imposta il riempimento specificato su una sfumatura a due colori. Si applica solo a Excel 2007. |

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
int seriesIndex = chart.NSeries.Add("A1:B4", true);
//Impostazione dell'origine dati per i dati di categoria di NSeries
chart.NSeries.CategoryData = "C1:C4";
//Riempendo l'area della 2a NSeries con un gradiente
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1);

[Visual Basic]

Creazione di un'istanza di un oggetto Workbook
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
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Impostazione dell'origine dati per i dati di categoria di NSeries
chart.NSeries.CategoryData = "C1:C4"
'Riempimento dell'area della 2a NSeries con un gradiente
chart.NSeries(seriesIndex).Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1)
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
