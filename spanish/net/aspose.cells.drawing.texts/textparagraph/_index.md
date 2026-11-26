---
title: "Clase TextParagraph"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.TextParagraph. Representa la configuración del párrafo de texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/
---
## TextParagraph class

Representa la configuración del párrafo de texto.

```csharp
public class TextParagraph : FontSetting
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing.texts/textparagraph/alignmenttype/) { get; set; } | Obtiene y establece el tipo de alineación horizontal del texto del párrafo. |
| [Bullet](../../aspose.cells.drawing.texts/textparagraph/bullet/) { get; } | Obtiene la viñeta. |
| [Children](../../aspose.cells.drawing.texts/textparagraph/children/) { get; } | Obtiene todas las ejecuciones de texto en este párrafo. Si este párrafo está vacío, devuelve el propio párrafo. |
| [DefaultTabSize](../../aspose.cells.drawing.texts/textparagraph/defaulttabsize/) { get; set; } | Obtiene y establece el tamaño predeterminado para un carácter de tabulación dentro de este párrafo. |
| [FirstLineIndent](../../aspose.cells.drawing.texts/textparagraph/firstlineindent/) { get; set; } | Especifica el tamaño de sangría que se aplicará a la primera línea de texto del párrafo. |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Devuelve la fuente de este objeto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [FontAlignType](../../aspose.cells.drawing.texts/textparagraph/fontaligntype/) { get; set; } | Determina dónde, verticalmente, en una línea de texto se posicionan las palabras reales. Esto trata sobre la colocación vertical de los caracteres con respecto a las líneas base. |
| [IsEastAsianLineBreak](../../aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/) { get; set; } | Especifica si una palabra de Asia Oriental puede dividirse a la mitad y pasar a la siguiente línea sin que se añada un guion. |
| [IsHangingPunctuation](../../aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/) { get; set; } | Especifica si la puntuación debe disponerse forzosamente en una línea de texto o colocarse en una línea de texto diferente. |
| [IsLatinLineBreak](../../aspose.cells.drawing.texts/textparagraph/islatinlinebreak/) { get; set; } | Especifica si una palabra latina puede dividirse a la mitad y pasar a la siguiente línea sin que se añada un guion. |
| [LeftMargin](../../aspose.cells.drawing.texts/textparagraph/leftmargin/) { get; set; } | Especifica el margen izquierdo del párrafo. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtiene la longitud de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LineSpace](../../aspose.cells.drawing.texts/textparagraph/linespace/) { get; set; } | Obtiene y establece la cantidad de espacio blanco vertical que se utilizará dentro de un párrafo. |
| [LineSpaceSizeType](../../aspose.cells.drawing.texts/textparagraph/linespacesizetype/) { get; set; } | Obtiene y establece la cantidad de espacio blanco vertical que se utilizará dentro de un párrafo. |
| [RightMargin](../../aspose.cells.drawing.texts/textparagraph/rightmargin/) { get; set; } | Especifica el margen derecho del párrafo. |
| [SpaceAfter](../../aspose.cells.drawing.texts/textparagraph/spaceafter/) { get; set; } | Obtiene y establece la cantidad de espacio en blanco vertical que estará presente después de un párrafo. |
| [SpaceAfterSizeType](../../aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/) { get; set; } | Obtiene y establece la cantidad de espacio en blanco vertical que estará presente después de un párrafo. |
| [SpaceBefore](../../aspose.cells.drawing.texts/textparagraph/spacebefore/) { get; set; } | Obtiene y establece la cantidad de espacio en blanco vertical que estará presente antes de un párrafo. |
| [SpaceBeforeSizeType](../../aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/) { get; set; } | Obtiene y establece la cantidad de espacio en blanco vertical que estará presente antes de un párrafo. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtiene el índice de inicio de los caracteres. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Stops](../../aspose.cells.drawing.texts/textparagraph/stops/) { get; } | Obtiene la lista de tabulaciones. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Devuelve las opciones de texto. (Heredado de [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.texts/textparagraph/type/) { get; } | Obtiene el tipo de nodo de texto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Establece el estilo WordArt predefinido.(Hereda de [`FontSetting`](../../aspose.cells/fontsetting/).) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            int textBoxIndex = sheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = sheet.TextBoxes[textBoxIndex];
            
            // Establece el contenido de texto con varios párrafos
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Accede y modifica los párrafos de texto
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                // Establece las propiedades del párrafo
                paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
                paragraph.LineSpace = 20;
                paragraph.AlignmentType = TextAlignmentType.Center;
            }

            // Guarda el libro de trabajo
            workbook.Save("TextParagraphDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


