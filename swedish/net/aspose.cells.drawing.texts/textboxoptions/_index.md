---
title: "Klass TextBoxOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.TextBoxOptions-klass. Representerar textalternativen för formen"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textboxoptions/
---
## TextBoxOptions class

Representerar textalternativen för figuren

```csharp
public class TextBoxOptions
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | Om text får flöda över formen. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | Returnerar den nedre marginalen i enheten punkter |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | Hämtar och anger den vänstra marginalen i enheten punkter. |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | Anger om formen ska storleksändras för att passa texten |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | Hämtar och anger den högra marginalen i enheten punkter. |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | Hämtar eller anger textriktningen inom ett givet textområde. Det motsvarar "Format Shape - Text Options - Text Box - Text direction" i Excel |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | Det motsvarar "Format Shape - Text Options - Text Box - Vertical Alignment" i Excel. |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | Hämtar och anger den övre marginalen i enheten punkter. |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | Anger textbrytning inom en form. Falskt - Ingen brytning sker i textområdet. Sant - Brytning sker i textområdet. |

### Exempel

```csharp

[C#]
//Instansiering av ett Workbook-objekt
Workbook workbook = new Workbook();
int index = workbook.Worksheets[0].TextBoxes.Add(0, 0, 350, 350);
Shape shape = workbook.Worksheets[0].TextBoxes[index];
shape.Text = "This is test.";

//utför din verksamhet

//Spara Excel-filen.
workbook.Save("exmaple.xlsx");
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


