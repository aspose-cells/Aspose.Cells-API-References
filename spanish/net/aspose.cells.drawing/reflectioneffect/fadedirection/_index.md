---
title: "ReflectionEffect.FadeDirection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ReflectionEffect. Obtiene y establece la dirección para desplazar la reflexión"
type: docs
url: /es/net/aspose.cells.drawing/reflectioneffect/fadedirection/
---
## ReflectionEffect.FadeDirection property

Obtiene y establece la dirección para desplazar la reflexión.

```csharp
public double FadeDirection { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyFadeDirectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para aplicar el efecto de reflexión
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Obtener el efecto de reflexión de la forma
            ReflectionEffect reflection = shape.Reflection;

            // Mostrar el valor actual de FadeDirection
            Console.WriteLine("Current FadeDirection value: " + reflection.FadeDirection);

            // Establecer nuevo valor de FadeDirection (90 grados)
            reflection.FadeDirection = 90;
            Console.WriteLine("New FadeDirection value: " + reflection.FadeDirection);

            // Configurar otras propiedades de reflexión para una mejor visibilidad
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            reflection.Distance = 10;

            // Guardar el libro de trabajo para ver el efecto
            workbook.Save("ReflectionEffectFadeDirectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


