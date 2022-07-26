---
title: LineFormat
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa todos los ajustes de la línea.
type: docs
weight: 2220
url: /es/net/aspose.cells.drawing/lineformat/
---
## LineFormat class

Representa todos los ajustes de la línea.

```csharp
public class LineFormat : FillFormat
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BeginArrowheadLength](../../aspose.cells.drawing/lineformat/beginarrowheadlength) { get; set; } | Obtiene y establece el tipo de longitud de flecha inicial de la línea. |
| [BeginArrowheadStyle](../../aspose.cells.drawing/lineformat/beginarrowheadstyle) { get; set; } | Obtiene y establece el tipo de flecha de inicio de la línea. |
| [BeginArrowheadWidth](../../aspose.cells.drawing/lineformat/beginarrowheadwidth) { get; set; } | Obtiene y establece el tipo de ancho de flecha inicial de la línea. |
| [CapType](../../aspose.cells.drawing/lineformat/captype) { get; set; } | Especifica las mayúsculas finales. |
| [CompoundType](../../aspose.cells.drawing/lineformat/compoundtype) { get; set; } | Especifica el tipo de línea compuesta. |
| [DashStyle](../../aspose.cells.drawing/lineformat/dashstyle) { get; set; } | Especifica el tipo de guión de línea. |
| [EndArrowheadLength](../../aspose.cells.drawing/lineformat/endarrowheadlength) { get; set; } | Obtiene y establece el tipo de longitud de flecha final de la línea. |
| [EndArrowheadStyle](../../aspose.cells.drawing/lineformat/endarrowheadstyle) { get; set; } | Obtiene y establece el tipo de flecha final de la línea. |
| [EndArrowheadWidth](../../aspose.cells.drawing/lineformat/endarrowheadwidth) { get; set; } | Obtiene y establece el tipo de ancho de flecha final de la línea. |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Obtiene y establece el tipo de relleno |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Devuelve el color de degradado 1 para el relleno especificado. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Devuelve el color de degradado 2 para el relleno especificado. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Devuelve el tipo de color degradado para el relleno especificado. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Devuelve el grado de degradado para el relleno especificado. Solo aplica para Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Obtiene[`GradientFill`](../fillformat/gradientfill) objeto. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Devuelve el estilo de degradado para el relleno especificado. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Devuelve la variante de degradado para el relleno especificado. Solo se aplica a Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Obtiene y establece los datos de la imagen de la imagen. |
| [JoinType](../../aspose.cells.drawing/lineformat/jointype) { get; set; } | Especifica el tipo de unión de línea. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Representa el patrón de visualización de un área. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Obtiene[`PatternFill`](../fillformat/patternfill) objeto. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Obtiene y establece el tipo de formato de imagen. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Devuelve el color predeterminado de degradado para el relleno especificado. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Obtiene y establece la escala del formato de imagen. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Obtiene[`SolidFill`](../fillformat/solidfill) objeto. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Representa el tipo de textura para el relleno especificado. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Obtiene[`TextureFill`](../fillformat/texturefill) objeto. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0,0 (opaco) a 1,0 (transparente). |
| [Weight](../../aspose.cells.drawing/lineformat/weight) { get; set; } | Obtiene o establece el peso de la línea en unidades de puntos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/lineformat/equals)(object) | Determina si esta instancia tiene el mismo valor que otra instancia especificada[`LineFormat`](../lineformat) objeto. |
| override [GetHashCode](../../aspose.cells.drawing/lineformat/gethashcode)() | Obtiene el código hash. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Establece el relleno especificado en un degradado de un color. Solo se aplica a Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Establece el relleno especificado en un degradado de color predeterminado. Solo se aplica a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, Color, GradientStyleType, int) | Establece el relleno especificado en un degradado de dos colores. Solo se aplica a Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Establece el relleno especificado en un degradado de dos colores. Solo se aplica a Excel 2007. |

### Ejemplos

```csharp

[C#]
// Instanciando un objeto Workbook
Workbook workbook = new Workbook();
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
Shape shape = shapes.AddRectangle(1, 0, 1, 0, 50, 100);
LineFormat lineFmt = shape.Line;

//haz tu negocio

```

### Ver también

* class [FillFormat](../fillformat)
* espacio de nombres [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
