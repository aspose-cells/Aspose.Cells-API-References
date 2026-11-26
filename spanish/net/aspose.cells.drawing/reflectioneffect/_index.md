---
title: "Clase ReflectionEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ReflectionEffect. Esta clase especifica un efecto de reflexión"
type: docs
url: /es/net/aspose.cells.drawing/reflectioneffect/
---
## ReflectionEffect class

Esta clase especifica un efecto de reflexión.

```csharp
public class ReflectionEffect
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Blur](../../aspose.cells.drawing/reflectioneffect/blur/) { get; set; } | Obtiene y establece el radio de desenfoque, en unidades de puntos. |
| [Direction](../../aspose.cells.drawing/reflectioneffect/direction/) { get; set; } | Obtiene y establece la dirección de la rampa de degradado alfa relativa a la propia forma. |
| [Distance](../../aspose.cells.drawing/reflectioneffect/distance/) { get; set; } | Obtiene y establece la distancia de la sombra, en unidades de puntos. |
| [FadeDirection](../../aspose.cells.drawing/reflectioneffect/fadedirection/) { get; set; } | Obtiene y establece la dirección para desplazar la reflexión. |
| [RotWithShape](../../aspose.cells.drawing/reflectioneffect/rotwithshape/) { get; set; } | Obtiene y establece si la reflexión debe rotar con la forma. |
| [Size](../../aspose.cells.drawing/reflectioneffect/size/) { get; set; } | Obtiene y establece la posición final (a lo largo de la rampa de degradado alfa) del valor alfa final, en unidades de porcentaje |
| [Transparency](../../aspose.cells.drawing/reflectioneffect/transparency/) { get; set; } | Obtiene y establece el grado de transparencia inicial de la reflexión como un valor de 0.0 (opaco) a 1.0 (claro). |
| [Type](../../aspose.cells.drawing/reflectioneffect/type/) { get; set; } | Obtiene y establece el efecto de reflexión predefinido. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Establecer propiedades del efecto de reflexión
            ReflectionEffect reflection = shape.Reflection;
            reflection.Size = 90;
            reflection.Blur = 30;
            reflection.Transparency = 0.5;
            reflection.Distance = 10;

            // Mostrar propiedades de la reflexión
            Console.WriteLine("Reflection Size: " + reflection.Size);
            Console.WriteLine("Reflection Blur: " + reflection.Blur);
            Console.WriteLine("Reflection Transparency: " + reflection.Transparency);
            Console.WriteLine("Reflection Distance: " + reflection.Distance);

            // Guarda el libro de trabajo
            workbook.Save("ReflectionEffectDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


