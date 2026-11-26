---
title: "Clase FillFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.FillFormat. Encapsula el objeto que representa el formato de relleno para una forma"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Encapsula el objeto que representa el formato de relleno para una forma.

```csharp
public class FillFormat
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype/) { get; set; } | Obtiene y establece el tipo de relleno |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1/) { get; } | Devuelve el color de degradado 1 para el relleno especificado. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2/) { get; } | Devuelve el color de degradado 2 para el relleno especificado. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype/) { get; } | Devuelve el tipo de color de degradado para el relleno especificado. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree/) { get; } | Devuelve el grado de degradado para el relleno especificado. Solo se aplica a Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill/) { get; } | Obtiene el objeto [`GradientFill`](./gradientfill/). |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle/) { get; } | Devuelve el estilo de degradado para el relleno especificado. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant/) { get; } | Devuelve la variante de degradado para el relleno especificado. Solo se aplica a Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata/) { get; set; } | Obtiene y establece los datos de la imagen. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern/) { get; set; } | Representa el patrón de visualización de un área. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill/) { get; } | Obtiene el objeto [`PatternFill`](./patternfill/). |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype/) { get; set; } | Obtiene y establece el tipo de formato de imagen. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor/) { get; } | Devuelve el color predefinido del degradado para el relleno especificado. |
| [Scale](../../aspose.cells.drawing/fillformat/scale/) { get; set; } | Obtiene y establece la escala del formato de imagen. |
| [SetType](../../aspose.cells.drawing/fillformat/settype/) { get; set; } | (**Obsoleto.**) Obtiene el tipo de conjunto de formato de relleno. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill/) { get; } | Obtiene el objeto [`SolidFill`](./solidfill/). |
| [Texture](../../aspose.cells.drawing/fillformat/texture/) { get; set; } | Representa el tipo de textura para el relleno especificado. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill/) { get; } | Obtiene el objeto [`TextureFill`](./texturefill/). |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro). |
| [Type](../../aspose.cells.drawing/fillformat/type/) { get; set; } | (**Obsoleto.**) Obtiene y establece el tipo de relleno. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode/)() | Obtiene el código hash. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Establece el relleno especificado a un degradado de un color. Solo se aplica a Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient/)(GradientPresetType, GradientStyleType, int) | Establece el relleno especificado a un degradado de color predefinido. Solo se aplica a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Establece el relleno especificado a un degradado de dos colores. Solo se aplica a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Establece el relleno especificado a un degradado de dos colores. Solo se aplica a Excel 2007. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");
            
            // Agregar un gráfico de columnas a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar series de datos al gráfico
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            
            // Aplicar degradado de relleno al área de la serie
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(System.Drawing.Color.Lime, 1, 
                GradientStyleType.Horizontal, 1);
            
            // Guarda el libro de trabajo
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


