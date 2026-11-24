---
title: "Class TextBoxOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.TextBoxOptions class. Stellt die Textoptionen der Form dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/textboxoptions/
---
## TextBoxOptions class

Stellt die Textoptionen der Form dar

```csharp
public class TextBoxOptions
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | Ob Text die Form überlaufen darf. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | Gibt den unteren Rand in Punkten zurück |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | Ermittelt und legt den linken Rand in der Einheit Punkte fest. |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | Gibt an, ob die Form an den Text angepasst werden soll. |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | Ermittelt und legt den rechten Rand in der Einheit Punkte fest. |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | Ermittelt oder legt die Textanzeigerichtung innerhalb eines gegebenen Textkörpers fest. Sie entspricht "Format Shape - Text Options - Text Box - Text direction" in Excel. |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | Entspricht "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | Ermittelt und legt den oberen Rand in der Einheit Punkte fest. |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | Gibt an, wie der Text in einer Form umbrochen wird. False - Es erfolgt kein Umbruch im Textkörper. True - Es erfolgt ein Umbruch im Textkörper. |

### Beispiele

```csharp

[C#]
//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();
int index = workbook.Worksheets[0].TextBoxes.Add(0, 0, 350, 350);
Shape shape = workbook.Worksheets[0].TextBoxes[index];
shape.Text = "This is test.";

//Erledigen Sie Ihr Geschäft.

//Speichern Sie die Excel-Datei.
workbook.Save("exmaple.xlsx");
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


