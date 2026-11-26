---
title: "ShapePath.CubicBezierTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapePath. Añade una curva Bézier cúbica a la figura actual. El punto de inicio es el punto final de la figura actual. Unidad píxel"
type: docs
url: /es/net/aspose.cells.drawing/shapepath/cubicbezierto/
---
## ShapePath.CubicBezierTo method

Añade una curva cúbica Bézier a la figura actual. El punto de inicio es el punto final de la figura actual. Unidad: Pixel.

```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, 
    float endY)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ctrX1 | Single | La coordenada x del primer punto de control de la curva (Unidad: píxel). |
| ctrY1 | Single | La coordenada y del primer punto de control de la curva (Unidad: píxel). |
| ctrX2 | Single | La coordenada x del segundo punto de control de la curva (Unidad: píxel). |
| ctrY2 | Single | La coordenada y del segundo punto de control de la curva (Unidad: píxel). |
| endX | Single | La coordenada x del punto final de la curva (Unidad: píxel). |
| endY | Single | La coordenada y del punto final de la curva (Unidad: píxel). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCubicBezierToWithSingleSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            //Crear una nueva ruta de forma
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                        96.5f, -7.148871f,
                        130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                        182.24997f, 75.351f,
                        201, 120.517795f);
            shapePath1.MoveTo(150, 70);
            shapePath1.ArcTo(25, 25, 0, 270);


            //agregar forma libre
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath1 });

            // Guardar el resultado
            workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


