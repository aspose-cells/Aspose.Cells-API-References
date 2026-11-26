---
title: "Clase ShapePathPoint"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ShapePathPoint. Especifica coordenadas de posición o marcadores de ángulo. Las coordenadas de posición representan las coordenadas de una ruta en un espacio de coordenadas, p. ej., X/Y. Los marcadores de ángulo indican cambios angulares en una ruta, p. ej., los ángulos de inicio y de arco."
type: docs
url: /es/net/aspose.cells.drawing/shapepathpoint/
---
## ShapePathPoint class

Especifique coordenadas de posición o marcadores de ángulo. Las coordenadas de posición representan las coordenadas de una ruta en un espacio de coordenadas (p. ej., X/Y). Los marcadores de ángulo indican cambios angulares en una ruta (p. ej., los ángulos de inicio y de arco).

```csharp
public class ShapePathPoint
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Type](../../aspose.cells.drawing/shapepathpoint/type/) { get; } | Especifica el tipo de valor del objeto actual. |
| [X](../../aspose.cells.drawing/shapepathpoint/x/) { get; set; } | (**Obsoleto.**) Obtiene y establece la coordenada x para esta coordenada de posición. Unidad EMUs. |
| [XAngle](../../aspose.cells.drawing/shapepathpoint/xangle/) { get; set; } | Cuando el objeto es un marcador de ángulo, obtenga o establezca el primer ángulo en grados. |
| [XPixel](../../aspose.cells.drawing/shapepathpoint/xpixel/) { get; set; } | Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada x en píxeles. |
| [Y](../../aspose.cells.drawing/shapepathpoint/y/) { get; set; } | (**Obsoleto.**) Obtiene la coordenada y para esta coordenada de posición. Unidad EMUs. |
| [YAngle](../../aspose.cells.drawing/shapepathpoint/yangle/) { get; set; } | Cuando el objeto es un marcador de ángulo, obtenga o establezca el segundo ángulo en grados. |
| [YPixel](../../aspose.cells.drawing/shapepathpoint/ypixel/) { get; set; } | Cuando el objeto es una coordenada de posición, obtenga o establezca la coordenada y en píxeles. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Agregar una forma que contenga puntos de ruta con todos los parámetros requeridos.
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);
                
                // Obtener los puntos de ruta de la geometría.
                CustomGeometry geometry = shape.Geometry as CustomGeometry;
                if (geometry != null && geometry.Paths.Count > 0)
                {
                    ShapePath path = geometry.Paths[0];
                    
                    // Acceder a un punto de ruta existente (si está disponible).
                    if (path.PathSegementList.Count > 0)
                    {
                        // Obtener el primer punto (la implementación real puede variar según el tipo de segmento).
                        ShapePathPoint point = path.PathSegementList[0].Points[0];
                        
                        // Mostrar las coordenadas del punto
                        Console.WriteLine($"ShapePathPoint at X: {point.X}, Y: {point.Y}");
                    }
                }
                
                // Guarda el libro de trabajo
                workbook.Save("ShapePathPointDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPoint: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


