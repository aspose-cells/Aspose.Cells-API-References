---
title: "Style.GetTwoColorGradientSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Obtener la configuración de degradado de dos colores"
type: docs
url: /es/net/aspose.cells/style/gettwocolorgradientsetting/
---
## Style.GetTwoColorGradientSetting method

Obtiene la configuración de degradado bicolor.

```csharp
public TwoColorGradient GetTwoColorGradientSetting()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class StyleMethodGetTwoColorGradientSettingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo y establecer un degradado de dos colores
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);
            style.IsGradient = true;

            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Two Color Gradient Demo");
            cell.SetStyle(style);

            try
            {
                // Llamar al método GetTwoColorGradientSetting
                TwoColorGradient gradientSetting = style.GetTwoColorGradientSetting();

                // Mostrar la configuración del degradado
                Console.WriteLine("Color1: " + gradientSetting.Color1);
                Console.WriteLine("Color2: " + gradientSetting.Color2);
                Console.WriteLine("GradientStyleType: " + gradientSetting.GradientStyleType);
                Console.WriteLine("Variant: " + gradientSetting.Variant);

                // Modificar la configuración del degradado
                gradientSetting.Color1 = Color.Green;
                gradientSetting.GradientStyleType = GradientStyleType.Vertical;
                style.SetTwoColorGradient(gradientSetting.Color1, gradientSetting.Color2, 
                                        gradientSetting.GradientStyleType, gradientSetting.Variant);

                Console.WriteLine("Gradient settings modified successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTwoColorGradientSetting method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("MethodGetTwoColorGradientSettingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TwoColorGradient](../../twocolorgradient/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


