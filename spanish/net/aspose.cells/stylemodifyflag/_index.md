---
title: "Enumeración StyleModifyFlag"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.StyleModifyFlag. Los indicadores de estilo modificado"
type: docs
url: /es/net/aspose.cells/stylemodifyflag/
---
## StyleModifyFlag enumeration

Los indicadores de estilo modificado.

```csharp
public enum StyleModifyFlag
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| LeftBorder | `256` | Indica si el borde izquierdo ha sido modificado para el estilo. |
| RightBorder | `512` | Indica si el borde derecho ha sido modificado para el estilo. |
| TopBorder | `1024` | Indica si el borde superior ha sido modificado para el estilo. |
| BottomBorder | `2048` | Indica si el borde inferior ha sido modificado para el estilo. |
| DiagonalDownBorder | `4096` | Indica si el borde diagonal descendente ha sido modificado para el estilo. |
| DiagonalUpBorder | `8192` | Indica si el borde diagonal ascendente ha sido modificado para el estilo. |
| HorizontalBorder | `32` | Indica si el borde horizontal ha sido modificado para el estilo. Solo para estilos dinámicos, como el formato condicional. |
| VerticalBorder | `64` | Indica si el borde vertical ha sido modificado para el estilo. Solo para estilos dinámicos, como el formato condicional. |
| SideBorders | `3840` | Indica los cuatro bordes laterales: LeftBorder, RightBorder, TopBorder y BottomBorder. |
| Diagonal | `12288` | Indica los bordes diagonales: DiagonalDownBorder y DiagonalUpBorder. |
| DynamicStyleBorders | `96` | Indica los bordes del estilo dinámico: HorizontalBorder y VerticalBorder. |
| Borders | `16224` | Indica si uno o más bordes (LeftBorder, RightBorder, TopBorder, BottomBorder, Diagonal, HorizontalBorder, VerticalBorder) han sido modificados para el estilo. |
| NumberFormat | `16384` | Indica si el formato numérico ha sido modificado. |
| HorizontalAlignment | `32768` | Indica si la alineación horizontal ha sido modificada. |
| VerticalAlignment | `65536` | Indica si la alineación vertical ha sido modificada. |
| Indent | `131072` | Indica si la propiedad de sangría ha sido modificada. |
| Rotation | `262144` | Indica si la propiedad de rotación ha sido modificada. |
| WrapText | `524288` | Indica si la propiedad de ajuste de texto ha sido modificada. |
| ShrinkToFit | `1048576` | Indica si la propiedad de encoger para ajustar ha sido modificada. |
| TextDirection | `2097152` | Indica si la propiedad de dirección del texto ha sido modificada. |
| RelativeIndent | `128` | Indica si la propiedad de sangría relativa ha sido modificada para el estilo. Solo para estilos dinámicos, como el formato condicional. |
| AlignmentSettings | `4161664` | Indica si una o más propiedades relacionadas con la alineación (HorizontalAlignment, VerticalAlignment, Rotation, WrapText, WrapText, Indent, ShrinkToFit, TextDirection, RelativeIndent) han sido modificadas. |
| Pattern | `4194304` | Indica si el patrón del sombreado ha sido modificado. |
| ForegroundColor | `8388608` | Indica si el color de primer plano ha sido modificado. |
| BackgroundColor | `16777216` | Indica si el color de fondo ha sido modificado. |
| CellShading | `29360128` | Indica si una o más propiedades relacionadas con el sombreado (Pattern, ForegroundColor, BackgroundColor) han sido modificadas. |
| Locked | `67108864` | Indica si la propiedad de bloqueo ha sido modificada. |
| HideFormula | `134217728` | Indica si la propiedad de ocultar fórmula ha sido modificada. |
| ProtectionSettings | `201326592` | Indica si una o más propiedades relacionadas con la protección (Locked, HideFormula) han sido modificadas. |
| FontSize | `1` | Indica si el tamaño de fuente ha sido modificado. |
| FontName | `2` | Indica si el nombre de fuente ha sido modificado. |
| FontColor | `3` | Indica si el color de fuente ha sido modificado. |
| FontWeight | `4` | Indica si el grosor de la fuente ha sido modificado. |
| FontItalic | `5` | Indica si la propiedad cursiva de la fuente ha sido modificada. |
| FontUnderline | `6` | Indica si la propiedad subrayado de la fuente ha sido modificada. |
| FontStrike | `7` | Indica si la propiedad tachado de la fuente ha sido modificada. |
| FontScript | `8` | Indica si la propiedad de subíndice o superíndice de la fuente ha sido modificada. |
| FontFamily | `9` | Indica si la familia de fuentes ha sido modificada. |
| FontCharset | `10` | Indica si el conjunto de caracteres de la fuente ha sido modificado. |
| FontScheme | `11` | no usado. |
| FontDirty | `12` | no usado. |
| FontSpellingError | `13` | no usado. |
| FontUFillTx | `14` | no usado. |
| FontSpacing | `15` | no usado. |
| FontKerning | `16` | no usado. |
| FontEqualize | `17` | no usado. |
| FontCap | `18` | no usado. |
| FontVerticalText | `19` |  |
| Font | `31` | Indica si una o más propiedades han sido modificadas para la fuente del estilo. |
| All | `234881023` | Todas las propiedades que pueden modificarse para el estilo. |
| None | `0` | No se ha especificado ninguna propiedad. |

### Observaciones

Se definen combinaciones de múltiples propiedades para la comodidad del usuario. Al comprobar si están modificadas para un estilo, el valor devuelto indica si una o más propiedades de la combinación han sido modificadas.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleModifyFlagDemo
    {
        public static void StyleModifyFlagExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer algunos valores en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A2"].PutValue(123.45);

            // Crear un nuevo estilo
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Color = System.Drawing.Color.Blue;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;

            // Aplicar el estilo a una celda
            worksheet.Cells["A1"].SetStyle(style);

            // Comprobar qué propiedades del estilo han sido modificadas
            bool isFontModified = style.IsModified(StyleModifyFlag.Font);
            bool isFontSizeModified = style.IsModified(StyleModifyFlag.FontSize);
            bool isFontColorModified = style.IsModified(StyleModifyFlag.FontColor);
            bool isHorizontalAlignmentModified = style.IsModified(StyleModifyFlag.HorizontalAlignment);

            // Genere la salida de los resultados
            Console.WriteLine("Font Modified: " + isFontModified);
            Console.WriteLine("Font Size Modified: " + isFontSizeModified);
            Console.WriteLine("Font Color Modified: " + isFontColorModified);
            Console.WriteLine("Horizontal Alignment Modified: " + isHorizontalAlignmentModified);

            // Guarda el libro de trabajo
            workbook.Save("StyleModifyFlagExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


