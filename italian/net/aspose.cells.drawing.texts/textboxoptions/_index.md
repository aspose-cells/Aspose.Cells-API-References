---
title: "Classe TextBoxOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Texts.TextBoxOptions. Rappresenta le opzioni di testo della forma"
type: docs
url: /it/net/aspose.cells.drawing.texts/textboxoptions/
---
## TextBoxOptions class

Rappresenta le opzioni di testo della forma

```csharp
public class TextBoxOptions
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | Se consentire al testo di traboccare dalla forma. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | Restituisce il margine inferiore in unità di punti |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | Ottiene e imposta il margine sinistro in unità di Punti. |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | Indica se ridimensionare la forma per adattarla al testo |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | Ottiene e imposta il margine destro in unità di Punti. |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | Ottiene o imposta la direzione di visualizzazione del testo all'interno di un determinato corpo di testo. Corrisponde a "Format Shape - Text Options - Text Box - Text direction" in Excel |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | Corrisponde a "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | Ottiene e imposta il margine superiore in unità di Punti. |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | Specifica l'adattamento del testo all'interno di una forma. False - Nessun adattamento avverrà sul corpo del testo. True - L'adattamento avverrà sul corpo del testo. |

### Esempi

```csharp

[C#]
//Istanziare un oggetto Workbook
Workbook workbook = new Workbook();
int index = workbook.Worksheets[0].TextBoxes.Add(0, 0, 350, 350);
Shape shape = workbook.Worksheets[0].TextBoxes[index];
shape.Text = "This is test.";

//esegui la tua attività

//Salva il file Excel.
workbook.Save("exmaple.xlsx");
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


