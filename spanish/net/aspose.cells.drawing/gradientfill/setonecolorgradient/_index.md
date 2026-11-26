---
title: "GradientFill.SetOneColorGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GradientFill. Establece el relleno especificado a un degradado de un solo color. Solo se aplica a Excel 2007"
type: docs
url: /es/net/aspose.cells.drawing/gradientfill/setonecolorgradient/
---
## GradientFill.SetOneColorGradient method

Establece el relleno especificado a un degradado de un color. Solo se aplica a Excel 2007.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | Color | Un color de degradado. |
| grado | Double | El grado del degradado. Puede ser un valor de 0.0 (oscuro) a 1.0 (claro). |
| estilo | GradientStyleType | Estilo de sombreado de degradado. |
| variant | Int32 | La variante del degradado. Puede ser un valor de 1 a 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para aplicar relleno degradado
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Establecer el tipo de relleno a degradado
                shape.Fill.FillType = FillType.Gradient;

                // Obtener el relleno degradado
                GradientFill gradientFill = shape.Fill.GradientFill;
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Llamar a SetOneColorGradient con parámetros realistas
                gradientFill.SetOneColorGradient(
                    Color.Green,        // color
                    0.7,                // degree (70% intensity)
                    GradientStyleType.DiagonalUp,  // style
                    1);                 // variant

                Console.WriteLine("SetOneColorGradient method called successfully with parameters (Green, 0.7, DiagonalUp, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }

            // Guarda el libro de trabajo para demostrar el efecto
            workbook.Save("SetOneColorGradientDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


