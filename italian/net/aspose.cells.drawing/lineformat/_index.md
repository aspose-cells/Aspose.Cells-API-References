---
title: LineFormat
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta tutte le impostazioni della linea.
type: docs
weight: 2220
url: /it/net/aspose.cells.drawing/lineformat/
---
## LineFormat class

Rappresenta tutte le impostazioni della linea.

```csharp
public class LineFormat : FillFormat
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BeginArrowheadLength](../../aspose.cells.drawing/lineformat/beginarrowheadlength) { get; set; } | Ottiene e imposta il tipo di lunghezza della freccia iniziale della linea. |
| [BeginArrowheadStyle](../../aspose.cells.drawing/lineformat/beginarrowheadstyle) { get; set; } | Ottiene e imposta il tipo di freccia di inizio della riga. |
| [BeginArrowheadWidth](../../aspose.cells.drawing/lineformat/beginarrowheadwidth) { get; set; } | Ottiene e imposta il tipo di larghezza della freccia iniziale della linea. |
| [CapType](../../aspose.cells.drawing/lineformat/captype) { get; set; } | Specifica le maiuscole finali. |
| [CompoundType](../../aspose.cells.drawing/lineformat/compoundtype) { get; set; } | Specifica il tipo di riga composta. |
| [DashStyle](../../aspose.cells.drawing/lineformat/dashstyle) { get; set; } | Specifica il tipo di trattino. |
| [EndArrowheadLength](../../aspose.cells.drawing/lineformat/endarrowheadlength) { get; set; } | Ottiene e imposta il tipo di lunghezza della freccia finale della linea. |
| [EndArrowheadStyle](../../aspose.cells.drawing/lineformat/endarrowheadstyle) { get; set; } | Ottiene e imposta il tipo di freccia finale della riga. |
| [EndArrowheadWidth](../../aspose.cells.drawing/lineformat/endarrowheadwidth) { get; set; } | Ottiene e imposta il tipo di larghezza della freccia finale della linea. |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Ottiene e imposta il tipo di riempimento |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Restituisce il colore della sfumatura 1 per il riempimento specificato. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Restituisce il colore della sfumatura 2 per il riempimento specificato. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Restituisce il tipo di colore sfumato per il riempimento specificato. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Restituisce il grado di sfumatura per il riempimento specificato. Vale solo per Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Ottiene[`GradientFill`](../fillformat/gradientfill) oggetto. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Restituisce lo stile del gradiente per il riempimento specificato. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Restituisce la variante del gradiente per il riempimento specificato. Vale solo per Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Ottiene e imposta i dati dell'immagine dell'immagine. |
| [JoinType](../../aspose.cells.drawing/lineformat/jointype) { get; set; } | Specifica il tipo di unione di linea. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Rappresenta il modello di visualizzazione di un'area. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Ottiene[`PatternFill`](../fillformat/patternfill) oggetto. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Ottiene e imposta il tipo di formato immagine. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Restituisce il colore predefinito del gradiente per il riempimento specificato. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Ottiene e imposta la scala del formato dell'immagine. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Ottiene[`SolidFill`](../fillformat/solidfill) oggetto. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Rappresenta il tipo di trama per il riempimento specificato. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Ottiene[`TextureFill`](../fillformat/texturefill) oggetto. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Restituisce o imposta il grado di trasparenza dell'area come un valore compreso tra 0,0 (opaco) e 1,0 (trasparente). |
| [Weight](../../aspose.cells.drawing/lineformat/weight) { get; set; } | Ottiene o imposta il peso della linea in unità di punti. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/lineformat/equals)(object) | Determina se questa istanza ha lo stesso valore di un'altra specificata[`LineFormat`](../lineformat) oggetto. |
| override [GetHashCode](../../aspose.cells.drawing/lineformat/gethashcode)() | Ottiene il codice hash. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Imposta il riempimento specificato su una sfumatura di un colore. Si applica solo a Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Imposta il riempimento specificato su una sfumatura di colore preimpostata. Si applica solo a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, Color, GradientStyleType, int) | Imposta il riempimento specificato su una sfumatura a due colori. Si applica solo a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Imposta il riempimento specificato su una sfumatura a due colori. Si applica solo a Excel 2007. |

### Esempi

```csharp

[C#]
//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
Shape shape = shapes.AddRectangle(1, 0, 1, 0, 50, 100);
LineFormat lineFmt = shape.Line;

//fai i tuoi affari

```

### Guarda anche

* class [FillFormat](../fillformat)
* spazio dei nomi [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
