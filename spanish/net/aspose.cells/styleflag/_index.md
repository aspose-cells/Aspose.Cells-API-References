---
title: "Clase StyleFlag"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.StyleFlag. Representa banderas que indican propiedades de formato aplicadas"
type: docs
url: /es/net/aspose.cells/styleflag/
---
## StyleFlag class

Representa indicadores que indican las propiedades de formato aplicadas.

```csharp
public class StyleFlag
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [StyleFlag](styleflag/)() | Construye un objeto con todas las banderas en falso. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Alignments](../../aspose.cells/styleflag/alignments/) { get; set; } | Se aplicará la configuración de alineación. |
| [All](../../aspose.cells/styleflag/all/) { get; set; } | Se aplicarán todas las propiedades. |
| [Borders](../../aspose.cells/styleflag/borders/) { get; set; } | Se aplicarán todas las configuraciones de bordes. |
| [BottomBorder](../../aspose.cells/styleflag/bottomborder/) { get; set; } | Se aplicarán las configuraciones del borde inferior. |
| [CellShading](../../aspose.cells/styleflag/cellshading/) { get; set; } | Se aplicará la configuración de sombreado de celda. |
| [DiagonalDownBorder](../../aspose.cells/styleflag/diagonaldownborder/) { get; set; } | Se aplicarán las configuraciones de borde diagonal descendente. |
| [DiagonalUpBorder](../../aspose.cells/styleflag/diagonalupborder/) { get; set; } | Se aplicarán las configuraciones de borde diagonal ascendente. |
| [Font](../../aspose.cells/styleflag/font/) { get; set; } | Se aplicarán las configuraciones de fuente. |
| [FontBold](../../aspose.cells/styleflag/fontbold/) { get; set; } | Se aplicará la configuración de negrita de fuente. |
| [FontColor](../../aspose.cells/styleflag/fontcolor/) { get; set; } | Se aplicará la configuración de color de fuente. |
| [FontItalic](../../aspose.cells/styleflag/fontitalic/) { get; set; } | Se aplicará la configuración de cursiva de fuente. |
| [FontName](../../aspose.cells/styleflag/fontname/) { get; set; } | Se aplicará la configuración del nombre de fuente. |
| [FontScript](../../aspose.cells/styleflag/fontscript/) { get; set; } | Se aplicará la configuración de script de fuente. |
| [FontSize](../../aspose.cells/styleflag/fontsize/) { get; set; } | Se aplicará la configuración de tamaño de fuente. |
| [FontStrike](../../aspose.cells/styleflag/fontstrike/) { get; set; } | Se aplicará la configuración de tachado de fuente. |
| [FontUnderline](../../aspose.cells/styleflag/fontunderline/) { get; set; } | Se aplicará la configuración de subrayado de fuente. |
| [HideFormula](../../aspose.cells/styleflag/hideformula/) { get; set; } | Se aplicará la configuración de ocultar fórmula. |
| [HorizontalAlignment](../../aspose.cells/styleflag/horizontalalignment/) { get; set; } | Se aplicará la configuración de alineación horizontal. |
| [Indent](../../aspose.cells/styleflag/indent/) { get; set; } | Se aplicará la configuración de nivel de sangría. |
| [LeftBorder](../../aspose.cells/styleflag/leftborder/) { get; set; } | Se aplicarán las configuraciones de borde izquierdo. |
| [Locked](../../aspose.cells/styleflag/locked/) { get; set; } | Se aplicará la configuración de bloqueo. |
| [NumberFormat](../../aspose.cells/styleflag/numberformat/) { get; set; } | Se aplicará la configuración de formato numérico. |
| [QuotePrefix](../../aspose.cells/styleflag/quoteprefix/) { get; set; } | Se aplicará la configuración de ocultar fórmula. |
| [RightBorder](../../aspose.cells/styleflag/rightborder/) { get; set; } | Se aplicarán las configuraciones de borde derecho. |
| [Rotation](../../aspose.cells/styleflag/rotation/) { get; set; } | Se aplicará la configuración de rotación. |
| [ShrinkToFit](../../aspose.cells/styleflag/shrinktofit/) { get; set; } | Se aplicará la configuración de reducir para ajustar. |
| [TextDirection](../../aspose.cells/styleflag/textdirection/) { get; set; } | Se aplicará la configuración de dirección de texto. |
| [TopBorder](../../aspose.cells/styleflag/topborder/) { get; set; } | Se aplicarán las configuraciones de borde superior. |
| [VerticalAlignment](../../aspose.cells/styleflag/verticalalignment/) { get; set; } | Se aplicará la configuración de alineación vertical. |
| [WrapText](../../aspose.cells/styleflag/wraptext/) { get; set; } | Se aplicará la configuración de ajuste de texto. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagDemo
    {
        public static void StyleFlagExample()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Header 1");
            worksheet.Cells["B1"].PutValue("Header 2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Crear un nuevo objeto de estilo
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Crear un nuevo objeto StyleFlag
            StyleFlag styleFlag = new StyleFlag
            {
                All = true,
                Font = true,
                FontSize = true,
                FontBold = true,
                CellShading = true
            };

            // Aplicar el estilo a un rango de celdas
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B1");
            range.ApplyStyle(style, styleFlag);

            // Guarda el libro de trabajo
            workbook.Save("StyleFlagExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


