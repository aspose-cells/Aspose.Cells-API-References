---
title: "Clase TextOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.TextOptions. Representa las opciones de texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/
---
## TextOptions class

Representa las opciones de texto.

```csharp
public class TextOptions : Font
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Obtiene y establece el color con un valor ARGB de 32 bits.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [CapsType](../../aspose.cells.drawing.texts/textoptions/capstype/) { get; set; } | Obtiene y establece el tipo de mayúsculas para los textos de la forma. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Representa el conjunto de caracteres.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [Color](../../aspose.cells/font/color/) { get; set; } | Obtiene o establece el color de la fuente.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Obtiene y establece el tamaño doble de la fuente.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [FarEastName](../../aspose.cells.drawing.texts/textoptions/fareastname/) { get; set; } | Obtiene y establece el nombre FarEast. |
| [Fill](../../aspose.cells.drawing.texts/textoptions/fill/) { get; } | Representa el formato de relleno del texto. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Obtiene o establece un valor que indica si la fuente está en negrita.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Obtiene o establece un valor que indica si la fuente está en cursiva.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [IsNormalizeHeights](../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/) { get; set; } | Indica si se debe aplicar la normalización de altura al tramo de texto. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Obtiene o establece un valor que indica si la fuente tiene un tachado simple.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Obtiene o establece un valor que indica si la fuente está en subíndice.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Obtiene o establece un valor que indica si la fuente está en superíndice.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [Kerning](../../aspose.cells.drawing.texts/textoptions/kerning/) { get; set; } | Especifica el tamaño mínimo de fuente en el que se aplicará el interletraje de caracteres para este tramo de texto. |
| [LanguageCode](../../aspose.cells.drawing.texts/textoptions/languagecode/) { get; set; } | Obtiene y establece el idioma de la interfaz de usuario. |
| [LatinName](../../aspose.cells.drawing.texts/textoptions/latinname/) { get; set; } | Obtiene y establece el nombre latino. |
| override [Name](../../aspose.cells.drawing.texts/textoptions/name/) { get; set; } | Obtiene y establece el nombre de la forma. |
| [Outline](../../aspose.cells.drawing.texts/textoptions/outline/) { get; } | Representa el formato de contorno del texto. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Obtiene y establece el tipo de esquema de la fuente.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Obtiene y establece el desplazamiento del script, en unidades de porcentaje(Hereda de [`Font`](../../aspose.cells/font/).) |
| [Shadow](../../aspose.cells.drawing.texts/textoptions/shadow/) { get; } | Representa un objeto [`ShadowEffect`](../../aspose.cells.drawing/shadoweffect/) que especifica el efecto de sombra para el elemento del gráfico o la forma. |
| [Size](../../aspose.cells/font/size/) { get; set; } | Obtiene o establece el tamaño de la fuente.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [Spacing](../../aspose.cells.drawing.texts/textoptions/spacing/) { get; set; } | Especifica el espaciado entre caracteres dentro de un tramo de texto. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Obtiene el tipo de tachado del texto.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Obtiene y establece el color del tema.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Obtiene o establece el tipo de subrayado de la fuente.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [UnderlineColor](../../aspose.cells.drawing.texts/textoptions/underlinecolor/) { get; set; } | Obtiene o establece el color del subrayado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/)(Font) | Comprueba si dos fuentes son iguales.(Hereda de [`Font`](../../aspose.cells/font/).) |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Establece el nombre y el esquema de la fuente.(Hereda de [`Font`](../../aspose.cells/font/).) |
| override [ToString](../../aspose.cells/font/tostring/)() | Devuelve una cadena que representa el objeto Cell actual.(Hereda de [`Font`](../../aspose.cells/font/).) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agrega una forma a la hoja de cálculo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            
            // Agrega texto a la forma y obtén TextOptions
            shape.TextBody.Text = "Sample Text";
            TextOptions textOptions = shape.TextBody[2].TextOptions;
            
            // Establece opciones de texto
            textOptions.Fill.SolidFill.Color = System.Drawing.Color.Red;
            textOptions.Fill.SolidFill.Transparency = 0.5;
            
            // Guarda el libro de trabajo
            workbook.Save("TextOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../../aspose.cells/font/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


