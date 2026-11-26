---
title: "GradientFill.SetGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GradientFill. Establece el tipo y la dirección del relleno de degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientfill/setgradient/
---
## GradientFill.SetGradient method

Establecer el tipo y la dirección del relleno degradado.

```csharp
public void SetGradient(GradientFillType type, double angle, GradientDirectionType direction)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | GradientFillType | Tipo de relleno de degradado. |
| angle | Double | El ángulo. Solo se aplica a GradientFillType.Linear. |
| direction | GradientDirectionType | El tipo de dirección. Solo se aplica a GradientFillType.Radial y GradientFillType.Rectangle. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GradientFillMethodSetGradientWithGradientFillTypeDoubleGradientDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma para aplicar relleno degradado
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 100);

            try
            {
                // Obtener el degradado de relleno de la forma
                GradientFill gradientFill = shape.Fill.GradientFill; // Fixed property name from Gradient to GradientFill
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Llamar a SetGradient con parámetros específicos: relleno lineal, 90 grados, dirección FromCenter
                gradientFill.SetGradient(GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter);
                
                Console.WriteLine("SetGradient method executed successfully with parameters (GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGradient method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo para demostrar el efecto
            workbook.Save("GradientFillSetGradientDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientFillType](../../gradientfilltype/)
* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


