---
title: "Enumeración MsoDrawingType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.MsoDrawingType. Representa el tipo de objetos de dibujo de Office"
type: docs
url: /es/net/aspose.cells.drawing/msodrawingtype/
---
## MsoDrawingType enumeration

Representa el tipo de objetos de dibujo de Office.

```csharp
public enum MsoDrawingType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Group | `0` | Grupo |
| Line | `1` | Línea |
| Rectangle | `2` | Rectángulo |
| Oval | `3` | Óvalo |
| Arc | `4` | Arco |
| Chart | `5` | Gráfico |
| TextBox | `6` | TextBox |
| Button | `7` | Botón |
| Picture | `8` | Imagen |
| Polygon | `9` | Polígono |
| CheckBox | `11` | CheckBox |
| RadioButton | `12` | RadioButton |
| Label | `14` | Etiqueta |
| DialogBox | `15` | DialogBox |
| Spinner | `16` | Spinner |
| ScrollBar | `17` | ScrollBar |
| ListBox | `18` | ListBox |
| GroupBox | `19` | GroupBox |
| ComboBox | `20` | ComboBox |
| Comment | `25` | Comentario |
| OleObject | `24` | OleObject |
| CellsDrawing | `30` | Solo para preservar el objeto de dibujo en el archivo de plantilla. |
| Unknown | `29` | Solo para preservar el objeto de dibujo en el archivo xlsx. |
| Slicer | `31` | Segmentador |
| WebExtension | `32` | Extensión web |
| SmartArt | `33` | Smart Art |
| CustomXml | `34` | Forma xml personalizada, como Ink. |
| Timeline | `35` | Línea de tiempo |
| Model3D | `36` | Modelo 3D |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma rectangular a la hoja de cálculo
            Shape rectangle = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 200);
            rectangle.Name = "MyRectangle";
            rectangle.AlternativeText = "This is a rectangle shape";

            // Agregar una forma ovalada a la hoja de cálculo
            Shape oval = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 5, 0, 5, 0, 100, 200);
            oval.Name = "MyOval";
            oval.AlternativeText = "This is an oval shape";

            // Agregar una forma de línea a la hoja de cálculo
            Shape line = worksheet.Shapes.AddShape(MsoDrawingType.Line, 8, 0, 8, 0, 100, 200);
            line.Name = "MyLine";
            line.AlternativeText = "This is a line shape";

            // Agregar una forma de cuadro de texto a la hoja de cálculo
            Shape textBox = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 11, 0, 11, 0, 100, 200);
            textBox.Name = "MyTextBox";
            textBox.AlternativeText = "This is a textbox shape";
            textBox.Text = "Hello, Aspose.Cells!";

            // Mostrar los nombres y tipos de las formas
            foreach (Shape shape in worksheet.Shapes)
            {
                Console.WriteLine($"Shape Name: {shape.Name}, Shape Type: {shape.MsoDrawingType}");
            }

            // Guarda el libro de trabajo
            workbook.Save("MsoDrawingTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


