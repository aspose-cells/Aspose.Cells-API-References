---
title: "Enum MsoDrawingType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.MsoDrawingType-enum. Representerar typ av kontorsritningsobjekt"
type: docs
url: /sv/net/aspose.cells.drawing/msodrawingtype/
---
## MsoDrawingType enumeration

Representerar typen av Office‑ritobjekt.

```csharp
public enum MsoDrawingType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Group | `0` | Grupp |
| Line | `1` | Linje |
| Rectangle | `2` | Rektangel |
| Oval | `3` | Oval |
| Arc | `4` | Båge |
| Chart | `5` | Diagram |
| TextBox | `6` | Textruta |
| Button | `7` | Knapp |
| Picture | `8` | Bild |
| Polygon | `9` | Polygon |
| CheckBox | `11` | Kryssruta |
| RadioButton | `12` | Radioknapp |
| Label | `14` | Etikett |
| DialogBox | `15` | Dialogruta |
| Spinner | `16` | Snurrkontroll |
| ScrollBar | `17` | Rullningslist |
| ListBox | `18` | Listruta |
| GroupBox | `19` | Gruppruta |
| ComboBox | `20` | Kombinationsruta |
| Comment | `25` | Kommentar |
| OleObject | `24` | Ole-objekt |
| CellsDrawing | `30` | Endast för att bevara ritobjektet i mallfilen. |
| Unknown | `29` | Endast för att bevara ritobjektet i xlsx-filen. |
| Slicer | `31` | Slicer |
| WebExtension | `32` | Webb-tillägg |
| SmartArt | `33` | SmartArt |
| CustomXml | `34` | Anpassad xml-form, till exempel Ink. |
| Timeline | `35` | Tidslinje |
| Model3D | `36` | 3D-modell |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoDrawingTypeDemo
    {
        public static void MsoDrawingTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform i arbetsbladet
            Shape rectangle = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);
            rectangle.Name = "MyRectangle";
            rectangle.AlternativeText = "This is a rectangle shape";

            // Lägg till en oval form i kalkylbladet
            Shape oval = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 5, 0, 5, 0, 100, 200);
            oval.Name = "MyOval";
            oval.AlternativeText = "This is an oval shape";

            // Lägg till en linjeform i arbetsbladet
            Shape line = worksheet.Shapes.AddShape(MsoDrawingType.Line, 8, 0, 8, 0, 100, 200);
            line.Name = "MyLine";
            line.AlternativeText = "This is a line shape";

            // Lägg till en textruteform i arbetsbladet
            Shape textBox = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 11, 0, 11, 0, 100, 200);
            textBox.Name = "MyTextBox";
            textBox.AlternativeText = "This is a textbox shape";
            textBox.Text = "Hello, Aspose.Cells!";

            // Skriv ut namnen och typerna på formerna
            foreach (Shape shape in worksheet.Shapes)
            {
                Console.WriteLine($"Shape Name: {shape.Name}, Shape Type: {shape.MsoDrawingType}");
            }

            // Spara arbetsboken
            workbook.Save("MsoDrawingTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


