---
title: "ReflectionEffect.Direction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ReflectionEffect. Obtiene y establece la dirección de la rampa de degradado alfa respecto a la propia forma"
type: docs
url: /es/net/aspose.cells.drawing/reflectioneffect/direction/
---
## ReflectionEffect.Direction property

Obtiene y establece la dirección de la rampa de degradado alfa relativa a la propia forma.

```csharp
public double Direction { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ReflectionEffectPropertyDirectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para aplicar el efecto de reflexión
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Obtener el efecto de reflexión de la forma
            ReflectionEffect reflection = shape.Reflection;
            
            // Mostrar el valor actual de Direction
            Console.WriteLine("Current Direction value: " + reflection.Direction);
            
            // Establecer nuevo valor de Direction (90 grados)
            reflection.Direction = 90;
            Console.WriteLine("New Direction value: " + reflection.Direction);
            
            // Configurar otras propiedades de reflexión para una mejor visibilidad
            reflection.Type = ReflectionEffectType.TightReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 50;
            reflection.Blur = 5;
            
            // Guardar el libro de trabajo para ver el efecto de reflexión
            workbook.Save("ReflectionEffectDirectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


