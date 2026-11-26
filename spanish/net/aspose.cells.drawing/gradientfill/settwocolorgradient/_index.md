---
title: "GradientFill.SetTwoColorGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GradientFill. Establece el relleno especificado a un degradado de dos colores. Solo se aplica a Excel 2007."
type: docs
url: /es/net/aspose.cells.drawing/gradientfill/settwocolorgradient/
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetTwoColorGradientWithColorColorGradientStyleTyInt32Demo
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

                // Llamar a SetTwoColorGradient con parámetros realistas
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    Color.Blue,         // color2
                    GradientStyleType.DiagonalDown,  // style
                    1);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, Blue, DiagonalDown, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Guarda el libro de trabajo para demostrar el efecto
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
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

    public class GradientFillMethodSetTwoColorGradientWithColorDoubleColorDoubleGradient297116Demo
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

                // Llamar a SetTwoColorGradient con parámetros realistas
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    0.5,                // transparency1 (50% transparent)
                    Color.Blue,         // color2
                    0.3,                // transparency2 (30% transparent)
                    GradientStyleType.Horizontal,  // style
                    2);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, 0.5, Blue, 0.3, Horizontal, 2)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Guarda el libro de trabajo para demostrar el efecto
            workbook.Save("SetTwoColorGradientWithTransparencyDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


