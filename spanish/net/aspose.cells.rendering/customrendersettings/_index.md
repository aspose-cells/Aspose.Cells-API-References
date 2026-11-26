---
title: "Clase CustomRenderSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.CustomRenderSettings. Representa configuraciones personalizadas durante el renderizado"
type: docs
url: /es/net/aspose.cells.rendering/customrendersettings/
---
## CustomRenderSettings class

Representa configuraciones personalizadas durante el renderizado.

```csharp
public class CustomRenderSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CustomRenderSettings](customrendersettings/)() | Ctor. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [GetCellBorderWidth](../../aspose.cells.rendering/customrendersettings/getcellborderwidth/)(CellBorderType) | Especifica el ancho del borde de la celda según el tipo de borde. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "Border Width Test";

            try
            {
                // Crea una instancia de CustomRenderSettings usando el constructor predeterminado
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Demuestra el método GetCellBorderWidth con diferentes tipos de borde
                float thinWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Muestra los resultados
                Console.WriteLine($"Thin border width: {thinWidth}");
                Console.WriteLine($"Thick border width: {thickWidth}");
                Console.WriteLine($"Dashed border width: {dashedWidth}");

                // Guarda el libro de trabajo
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("CustomRenderSettings demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CustomRenderSettings demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


