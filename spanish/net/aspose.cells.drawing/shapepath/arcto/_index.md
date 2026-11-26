---
title: "ShapePath.ArcTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapePath. Añade un arco elíptico a la figura actual. El punto de inicio es el punto final de la figura actual"
type: docs
url: /es/net/aspose.cells.drawing/shapepath/arcto/
---
## ShapePath.ArcTo method

Añade un arco elíptico a la figura actual. El punto de inicio es el punto final de la figura actual.

```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| wR | Single | La mitad del ancho del área rectangular de la elipse que dibuja el arco (Unidad: píxel). |
| hR | Single | La mitad de la altura del área rectangular de la elipse que dibuja el arco (Unidad: píxel). |
| stAng | Single | El ángulo de inicio del arco, medido en grados en sentido horario desde el eje x (Unidad: grado). Este ángulo especificará qué ángulo a lo largo de la supuesta trayectoria circular se usará como posición inicial para dibujar el arco. Este ángulo de inicio se bloqueará en la última posición conocida del lápiz en la ruta ShapePath. Así se garantiza una ruta continua. |
| swAng | Single | El ángulo de giro para un arco. Este ángulo especificará hasta qué punto, en términos de ángulo, a lo largo de la supuesta trayectoria circular, se extenderá el arco. La extensión desde el ángulo de inicio siempre será en sentido horario alrededor del círculo supuesto. (Unidad: grado) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodArcToWithSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            //Crear una nueva ruta de forma
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);

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

            Workbook workbook = new Workbook();

            //agregar forma libre
            workbook.Worksheets[0].Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath, shapePath1 });

            // Guardar el resultado
            workbook.Save("ShapePathMethodArcToDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


