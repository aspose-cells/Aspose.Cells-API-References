---
title: "FillFormat.SetTwoColorGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FillFormat. Establece el relleno especificado a un degradado de dos colores. Solo se aplica a Excel 2007"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/settwocolorgradient/
---
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}

Establece el relleno especificado a un degradado de dos colores. Solo se aplica a Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color1 | Color | Un color de degradado. |
| color2 | Color | Dos colores de degradado. |
| estilo | GradientStyleType | Estilo de sombreado de degradado. |
| variant | Int32 | La variante del degradado. Puede ser un valor de 1 a 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma simple para demostrar el relleno de degradado
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 100, 100);

            // Obtener el formato de relleno de la forma
            FillFormat fillFormat = shape.Fill;

            // Establecer degradado de dos colores con los parámetros especificados
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);

            // Guarda el libro de trabajo
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}

Establece el relleno especificado a un degradado de dos colores. Solo se aplica a Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2, 
    double transparency2, GradientStyleType style, int variant)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color1 | Color | Un color de degradado. |
| transparency1 | Double | El grado de transparencia del color1 como un valor de 0.0 (opaco) a 1.0 (transparente). |
| color2 | Color | Dos colores de degradado. |
| transparency2 | Double | El grado de transparencia del color2 como un valor de 0.0 (opaco) a 1.0 (transparente). |
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

    public class FillFormatMethodSetTwoColorGradientWithColorDoubleColorDoubleGradientDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma rectangular para demostrar el formato de relleno
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 150, 100);
            FillFormat fillFormat = rectangle.Fill;

            try
            {
                // Preparar parámetros para SetTwoColorGradient
                Color color1 = Color.Red;
                double transparency1 = 0.3;
                Color color2 = Color.Blue;
                double transparency2 = 0.7;
                GradientStyleType gradientStyle = GradientStyleType.Horizontal;
                int variant = 1;

                // Llamar a SetTwoColorGradient con parámetros específicos
                fillFormat.SetTwoColorGradient(
                    color1, 
                    transparency1, 
                    color2, 
                    transparency2, 
                    gradientStyle, 
                    variant
                );

                Console.WriteLine("SetTwoColorGradient executed successfully with parameters (Color, Double, Color, Double, GradientStyleType, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTwoColorGradient: {ex.Message}");
            }

            // Guardar el libro de trabajo para mostrar el efecto
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


