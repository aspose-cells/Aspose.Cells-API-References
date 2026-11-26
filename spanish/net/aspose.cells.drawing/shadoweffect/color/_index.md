---
title: "ShadowEffect.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShadowEffect. Obtiene y establece el color de la sombra"
type: docs
url: /es/net/aspose.cells.drawing/shadoweffect/color/
---
## ShadowEffect.Color property

Obtiene y establece el color de la sombra.

```csharp
public CellsColor Color { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShadowEffectPropertyColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular para demostrar el efecto de sombra
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Obtener el efecto de sombra de la forma
                ShadowEffect shadowEffect = shape.ShadowEffect;

                // Crear un nuevo objeto CellsColor
                CellsColor shadowColor = workbook.CreateCellsColor();

                // Establecer el color a rojo usando valores RGB
                shadowColor.Color = Color.Red;

                // Aplicar el color al efecto de sombra
                shadowEffect.Color = shadowColor;

                // Mostrar el valor actual del color
                Console.WriteLine("Shadow Color (RGB): " + shadowEffect.Color.Color.ToString());
                Console.WriteLine("Shadow Color (ARGB): " + shadowEffect.Color.Argb);

                // Guarda el libro de trabajo para demostrar el efecto
                workbook.Save("ShadowEffectColorDemo.xlsx");

                // Cargar el libro de trabajo nuevamente para verificar que el color se guardó
                Workbook loadedWorkbook = new Workbook("ShadowEffectColorDemo.xlsx");
                ShadowEffect loadedShadowEffect = loadedWorkbook.Worksheets[0].Shapes[0].ShadowEffect;

                // Mostrar el valor del color cargado
                Console.WriteLine("Loaded Shadow Color (RGB): " + loadedShadowEffect.Color.Color.ToString());
                Console.WriteLine("Loaded Shadow Color (ARGB): " + loadedShadowEffect.Color.Argb);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


