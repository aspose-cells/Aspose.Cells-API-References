---
title: "Clase Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Font. Encapsula el objeto de fuente usado en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/font/
---
## Font class

Encapsula el objeto de fuente usado en una hoja de cálculo.

```csharp
public class Font
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Obtiene y establece el color con un valor ARGB de 32 bits. |
| [CapsType](../../aspose.cells/font/capstype/) { get; set; } | (**Obsolete.**) Obtiene y establece el tipo de mayúsculas de texto. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Representa el conjunto de caracteres. |
| [Color](../../aspose.cells/font/color/) { get; set; } | Obtiene o establece el Color de la fuente. |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Obtiene y establece el doble tamaño de la fuente. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Obtiene o establece un valor que indica si la fuente está en negrita. |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Obtiene o establece un valor que indica si la fuente está en cursiva. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights/) { get; set; } | (**Obsoleto.**) Indica si la normalización de altura que se aplicará al fragmento de texto. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Obtiene o establece un valor que indica si la fuente tiene tachado simple. |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Obtiene o establece un valor que indica si la fuente está en subíndice. |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Obtiene o establece un valor que indica si la fuente está en superíndice. |
| virtual [Name](../../aspose.cells/font/name/) { get; set; } | Obtiene o establece el nombre del `Font`. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Obtiene y establece el tipo de esquema de la fuente. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Obtiene y establece el desplazamiento del script,en unidad de porcentaje |
| [Size](../../aspose.cells/font/size/) { get; set; } | Obtiene o establece el tamaño de la fuente. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Obtiene el tipo de tachado del texto. |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Obtiene y establece el color del tema. |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Obtiene o establece el tipo de subrayado de la fuente. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/#equals)(Font) | Comprueba si dos fuentes son iguales. |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Establece el nombre y el esquema de la fuente. |
| override [ToString](../../aspose.cells/font/tostring/)() | Devuelve una cadena que representa el objeto Cell actual. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontDemo
    {
        public static void FontExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[0];

            // Accediendo a la celda "A1" de la hoja de cálculo
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Añadiendo un valor a la celda "A1"
            cell.PutValue("Hello Aspose!");

            // Accediendo al objeto de fuente del estilo de celda
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Estableciendo el nombre de la fuente a "Times New Roman"
            font.Name = "Times New Roman";

            // Estableciendo el tamaño de la fuente a 14
            font.Size = 14;

            // Estableciendo el color de la fuente como Rojo
            font.Color = Color.Red;

            // Estableciendo propiedades adicionales de la fuente
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;
            font.IsStrikeout = false;
            font.IsSuperscript = false;
            font.IsSubscript = false;
            font.Charset = 1;
            font.CapsType = TextCapsType.None;
            font.StrikeType = TextStrikeType.None;
            font.ScriptOffset = 0;
            font.DoubleSize = 14.0;
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            font.ArgbColor = Color.Red.ToArgb();
            font.IsNormalizeHeights = false;
            font.SchemeType = FontSchemeType.None;

            // Guardando el archivo Excel
            workbook.Save("FontExample.xlsx");
            workbook.Save("FontExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


