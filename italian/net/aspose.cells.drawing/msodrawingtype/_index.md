---
title: "Enum MsoDrawingType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.MsoDrawingType. Rappresenta il tipo di oggetti di disegno Office"
type: docs
url: /it/net/aspose.cells.drawing/msodrawingtype/
---
## MsoDrawingType enumeration

Rappresenta il tipo di oggetti di disegno Office.

```csharp
public enum MsoDrawingType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Group | `0` | Gruppo |
| Line | `1` | Linea |
| Rectangle | `2` | Rettangolo |
| Oval | `3` | Ovale |
| Arc | `4` | Arco |
| Chart | `5` | Grafico |
| TextBox | `6` | TextBox |
| Button | `7` | Pulsante |
| Picture | `8` | Immagine |
| Polygon | `9` | Poligono |
| CheckBox | `11` | CheckBox |
| RadioButton | `12` | RadioButton |
| Label | `14` | Etichetta |
| DialogBox | `15` | DialogBox |
| Spinner | `16` | Spinner |
| ScrollBar | `17` | ScrollBar |
| ListBox | `18` | ListBox |
| GroupBox | `19` | GroupBox |
| ComboBox | `20` | ComboBox |
| Comment | `25` | Commento |
| OleObject | `24` | OleObject |
| CellsDrawing | `30` | Solo per preservare l'oggetto di disegno nel file modello. |
| Unknown | `29` | Solo per preservare l'oggetto di disegno nel file xlsx. |
| Slicer | `31` | Slicer |
| WebExtension | `32` | Estensione web |
| SmartArt | `33` | Smart Art |
| CustomXml | `34` | Forma xml personalizzata, ad esempio Ink. |
| Timeline | `35` | Cronologia |
| Model3D | `36` | Modello 3D |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare al foglio di lavoro
            Shape rectangle = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);
            rectangle.Name = "MyRectangle";
            rectangle.AlternativeText = "This is a rectangle shape";

            // Aggiungi una forma ovale al foglio di lavoro
            Shape oval = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 5, 0, 5, 0, 100, 200);
            oval.Name = "MyOval";
            oval.AlternativeText = "This is an oval shape";

            // Aggiungi una forma linea al foglio di lavoro
            Shape line = worksheet.Shapes.AddShape(MsoDrawingType.Line, 8, 0, 8, 0, 100, 200);
            line.Name = "MyLine";
            line.AlternativeText = "This is a line shape";

            // Aggiungi una forma casella di testo al foglio di lavoro
            Shape textBox = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 11, 0, 11, 0, 100, 200);
            textBox.Name = "MyTextBox";
            textBox.AlternativeText = "This is a textbox shape";
            textBox.Text = "Hello, Aspose.Cells!";

            // Restituisci i nomi e i tipi delle forme
            foreach (Shape shape in worksheet.Shapes)
            {
                Console.WriteLine($"Shape Name: {shape.Name}, Shape Type: {shape.MsoDrawingType}");
            }

            // Salva la cartella di lavoro
            workbook.Save("MsoDrawingTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


