---
title: "Style.GetTwoColorGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Obtener la configuración de degradado de dos colores"
type: docs
url: /es/net/aspose.cells/style/gettwocolorgradient/
---
## Style.GetTwoColorGradient method

Obtiene la configuración de degradado bicolor.

```csharp
[Obsolete("Use Style.GetTwoColorGradientSetting() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GetTwoColorGradient(out Color color1, out Color color2, 
    out GradientStyleType gradientStyleType, out int variant)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color1 | Color& | Un color de degradado. |
| color2 | Color& | Dos colores de degradado. |
| gradientStyleType | GradientStyleType& | Estilo de sombreado de degradado. |
| variant | Int32& | La variante del degradado. |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método Style.GetTwoColorGradientSetting(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class StyleMethodGetTwoColorGradientWithColorColorGradientStyleTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo y establecer un degradado de dos colores
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);

            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Two Color Gradient Demo");

            // Preparar variables para obtener la configuración del degradado
            Color color1 = Color.Empty;
            Color color2 = Color.Empty;
            GradientStyleType gradientStyle = GradientStyleType.Horizontal;
            int variant = 0;

            try
            {
                // Llamar al método GetTwoColorGradient
#pragma warning disable CS0618 // Type or member is obsolete
                style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);
#pragma warning restore CS0618 // Type or member is obsolete

                // Mostrar la configuración del degradado recuperada
                Console.WriteLine("Gradient Settings:");
                Console.WriteLine($"Color1: {color1}");
                Console.WriteLine($"Color2: {color2}");
                Console.WriteLine($"Gradient Style: {gradientStyle}");
                Console.WriteLine($"Variant: {variant}");

                // Guarda el libro de trabajo
                workbook.Save("StyleMethodGetTwoColorGradientDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTwoColorGradient method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


