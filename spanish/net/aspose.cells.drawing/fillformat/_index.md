---
title: FillFormat
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula el objeto que representa el formato de relleno para una forma.
type: docs
weight: 1970
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
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Obtiene y establece el tipo de relleno |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Devuelve el color de degradado 1 para el relleno especificado. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Devuelve el color de degradado 2 para el relleno especificado. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Devuelve el tipo de color degradado para el relleno especificado. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Devuelve el grado de degradado para el relleno especificado. Solo aplica para Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Obtiene[`GradientFill`](./gradientfill) objeto. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Devuelve el estilo de degradado para el relleno especificado. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Devuelve la variante de degradado para el relleno especificado. Solo se aplica a Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Obtiene y establece los datos de la imagen de la imagen. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Representa el patrón de visualización de un área. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Obtiene[`PatternFill`](./patternfill) objeto. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Obtiene y establece el tipo de formato de imagen. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Devuelve el color predeterminado de degradado para el relleno especificado. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Obtiene y establece la escala del formato de imagen. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Obtiene[`SolidFill`](./solidfill) objeto. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Representa el tipo de textura para el relleno especificado. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Obtiene[`TextureFill`](./texturefill) objeto. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0,0 (opaco) a 1,0 (transparente). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode)() | Obtiene el código hash. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Establece el relleno especificado en un degradado de un color. Solo se aplica a Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Establece el relleno especificado en un degradado de color predeterminado. Solo se aplica a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Establece el relleno especificado en un degradado de dos colores. Solo se aplica a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Establece el relleno especificado en un degradado de dos colores. Solo se aplica a Excel 2007. |

### Ejemplos

```csharp

[C#]

// Instanciando un objeto Workbook
Workbook workbook = new Workbook();
//Agregar una nueva hoja de cálculo al objeto de Excel
int sheetIndex = workbook.Worksheets.Add();
//Obteniendo la referencia de la hoja de trabajo recién agregada pasando su índice de hoja
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Agregar un valor de muestra a la celda "A1"
worksheet.Cells["A1"].PutValue(50);
// Agregar un valor de muestra a la celda "A2"
worksheet.Cells["A2"].PutValue(100);
// Agregar un valor de muestra a la celda "A3"
worksheet.Cells["A3"].PutValue(150);
// Agregar un valor de muestra a la celda "A4"
worksheet.Cells["A4"].PutValue(200);
// Agregar un valor de muestra a la celda "B1"
worksheet.Cells["B1"].PutValue(60);
// Agregar un valor de muestra a la celda "B2"
worksheet.Cells["B2"].PutValue(32);
// Agregar un valor de muestra a la celda "B3"
worksheet.Cells["B3"].PutValue(50);
// Agregar un valor de muestra a la celda "B4"
worksheet.Cells["B4"].PutValue(40);
// Agregar un valor de muestra a la celda "C1" como datos de categoría
worksheet.Cells["C1"].PutValue("Q1");
// Agregar un valor de muestra a la celda "C2" como datos de categoría
worksheet.Cells["C2"].PutValue("Q2");
// Agregar un valor de muestra a la celda "C3" como datos de categoría
worksheet.Cells["C3"].PutValue("Y1");
// Agregar un valor de muestra a la celda "C4" como datos de categoría
worksheet.Cells["C4"].PutValue("Y2");
//Añadiendo un gráfico a la hoja de trabajo
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accediendo a la instancia del gráfico recién agregado
Chart chart = worksheet.Charts[chartIndex];
// Agregar NSeries (fuente de datos del gráfico) al gráfico que va desde la celda "A1" hasta la celda "B4"
int seriesIndex = chart.NSeries.Add("A1:B4", true);
//Configuración de la fuente de datos para la categoría de datos de NSeries
chart.NSeries.CategoryData = "C1:C4";
//Rellenando el área de la 2nd NSeries con un degradado
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1);

[Visual Basic]

Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()
'Agregar una nueva hoja de cálculo al objeto de Excel
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Obtener la referencia de la hoja de trabajo recién agregada pasando su índice de hoja
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Adición de un gráfico a la hoja de cálculo
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Acceso a la instancia del gráfico recién agregado
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Configuración de la fuente de datos para los datos de categoría de NSeries
chart.NSeries.CategoryData = "C1:C4"
'Rellenar el área de la segunda serie N con un degradado
chart.NSeries(seriesIndex).Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1)
```

### Ver también

* espacio de nombres [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
