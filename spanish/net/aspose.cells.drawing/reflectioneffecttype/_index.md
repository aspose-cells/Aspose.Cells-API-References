---
title: "Enum ReflectionEffectType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ReflectionEffectType enum. Representa el tipo de efecto de reflexión"
type: docs
url: /es/net/aspose.cells.drawing/reflectioneffecttype/
---
## ReflectionEffectType enumeration

Representa el tipo de efecto de reflexión.

```csharp
public enum ReflectionEffectType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin efecto de reflexión. |
| Custom | `1` | Efecto de reflexión personalizado. |
| TightReflectionTouching | `2` | Reflexión ajustada, tocando. |
| HalfReflectionTouching | `3` | Reflexión a mitad, tocando. |
| FullReflectionTouching | `4` | Reflexión completa, tocando. |
| TightReflection4PtOffset | `5` | Reflexión ajustada, desplazamiento de 4 pt. |
| HalfReflection4PtOffset | `6` | Reflexión a mitad, desplazamiento de 4 pt. |
| FullReflection4PtOffset | `7` | Reflexión completa, desplazamiento de 4 pt. |
| TightReflection8PtOffset | `8` | Reflexión ajustada, desplazamiento de 8 pt. |
| HalfReflection8PtOffset | `9` | Reflexión a mitad, desplazamiento de 8 pt. |
| FullReflection8PtOffset | `10` | Reflexión completa, desplazamiento de 8 pt. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassReflectionEffectTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma rectangular
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            
            // Obtener el efecto de reflexión
            ReflectionEffect reflection = rectangle.Reflection;
            
            // Establecer propiedades de reflexión
            reflection.Type = ReflectionEffectType.HalfReflectionTouching;
            reflection.Transparency = 0.5;
            reflection.Size = 55;
            reflection.Blur = 0.5;
            reflection.Distance = 0;
            
            // Guarda el libro de trabajo
            workbook.Save("DrawingClassReflectionEffectTypeDemo.xlsx");
            
            Console.WriteLine("Reflection effect demo completed successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


