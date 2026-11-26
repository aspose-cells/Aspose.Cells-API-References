---
title: "Enumeración TextVerticalType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.Texts.TextVerticalType. Representa el tipo de dirección del texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textverticaltype/
---
## TextVerticalType enumeration

Representa el tipo de dirección del texto.

```csharp
public enum TextVerticalType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Vertical | `0` | Visualización vertical de Asia Oriental. |
| Horizontal | `1` | Texto horizontal. |
| VerticalLeftToRight | `2` | Se muestra vertical y el texto fluye de arriba a abajo y luego de IZQUIERDA a DERECHA |
| Vertical90 | `3` | Cada línea está rotada 90 grados en sentido horario |
| Vertical270 | `4` | Cada línea está rotada 270 grados en sentido horario |
| Stacked | `5` | Determina si todo el texto es vertical |
| StackedRightToLeft | `6` | Especifica que el WordArt vertical debe mostrarse de derecha a izquierda en lugar de izquierda a derecha. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextVerticalTypeDemo
    {
        public static void TextVerticalTypeExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Accediendo a la configuración de alineación de texto de la forma
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Estableciendo el tipo de verticalidad del texto a Horizontal
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Estableciendo otras propiedades para demostración
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
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
            workbook.Save("TextVerticalTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


