---
title: "Clase ShapeTextAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.ShapeTextAlignment. Representa la configuración de la alineación del texto de las formas"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/
---
## ShapeTextAlignment class

Representa la configuración de alineación de texto de la forma;

```csharp
public class ShapeTextAlignment
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing.texts/shapetextalignment/autosize/) { get; set; } | Indica si el tamaño de la forma se ajusta automáticamente según su contenido. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/bottommarginpt/) { get; set; } | Devuelve el margen inferior en unidades de puntos |
| [IsAutoMargin](../../aspose.cells.drawing.texts/shapetextalignment/isautomargin/) { get; set; } | Indica si el margen del marco de texto es automático. |
| [IsLockedText](../../aspose.cells.drawing.texts/shapetextalignment/islockedtext/) { get; set; } | Indica si la forma está bloqueada cuando la hoja de cálculo está protegida. |
| [IsTextWrapped](../../aspose.cells.drawing.texts/shapetextalignment/istextwrapped/) { get; set; } | Obtiene o establece el tipo de ajuste de texto de la forma que contiene texto. |
| [LeftMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/) { get; set; } | Devuelve el margen izquierdo en unidades de puntos |
| [NumberOfColumns](../../aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/) { get; set; } | Obtiene y establece el número de columnas de texto en el rectángulo delimitador. |
| [RightMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/) { get; set; } | Devuelve el margen derecho en unidades de puntos |
| [RotateTextWithShape](../../aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/) { get; set; } | Indica si se rota el texto con la forma. |
| [RotationAngle](../../aspose.cells.drawing.texts/shapetextalignment/rotationangle/) { get; set; } | Obtiene y establece la rotación de la forma. |
| [TextHorizontalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/) { get; set; } | Obtiene y establece el tipo de desbordamiento horizontal del texto del cuadro de texto. |
| [TextShapeType](../../aspose.cells.drawing.texts/shapetextalignment/textshapetype/) { get; set; } | Obtiene y establece el tipo de transformación del texto. |
| [TextVerticalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/) { get; set; } | Obtiene y establece el tipo de desbordamiento vertical del texto del cuadro de texto. |
| [TextVerticalType](../../aspose.cells.drawing.texts/shapetextalignment/textverticaltype/) { get; set; } | Obtiene y establece la dirección del texto. |
| [TopMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/topmarginpt/) { get; set; } | Devuelve el margen superior en unidades de puntos |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing.texts/shapetextalignment/equals/)(object) | Determina si esta instancia tiene el mismo valor que otro objeto `ShapeTextAlignment` especificado. |
| override [GetHashCode](../../aspose.cells.drawing.texts/shapetextalignment/gethashcode/)() |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class ShapeTextAlignmentDemo
    {
        public static void ShapeTextAlignmentExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Accediendo al objeto ShapeTextAlignment
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Estableciendo propiedades
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;
            shapeTextAlignment.IsLockedText = false;
            shapeTextAlignment.AutoSize = false;
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;
            shapeTextAlignment.TopMarginPt = 2.0d;
            shapeTextAlignment.BottomMarginPt = 2.0d;
            shapeTextAlignment.LeftMarginPt = 2.0d;
            shapeTextAlignment.RightMarginPt = 2.0d;
            shapeTextAlignment.IsAutoMargin = true;
            shapeTextAlignment.NumberOfColumns = 1;

            // Guardando el libro de trabajo
            workbook.Save("ShapeTextAlignmentExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


