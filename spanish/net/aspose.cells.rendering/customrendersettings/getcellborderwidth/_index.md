---
title: "CustomRenderSettings.GetCellBorderWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de CustomRenderSettings. Especifica el ancho del borde de la celda según el tipo de borde"
type: docs
url: /es/net/aspose.cells.rendering/customrendersettings/getcellborderwidth/
---
## CustomRenderSettings.GetCellBorderWidth method

Especifica el ancho del borde de la celda según el tipo de borde.

```csharp
public virtual float GetCellBorderWidth(CellBorderType borderType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderType | CellBorderType | tipo de borde de celda |

### Valor de retorno

ancho del borde de celda

### Observaciones

Cualquier valor negativo será ignorado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodGetCellBorderWidthWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea una instancia de CustomRenderSettings
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Llama a GetCellBorderWidth con diferentes tipos de borde
                float thinBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Muestra los resultados
                Console.WriteLine($"Thin border width: {thinBorderWidth}");
                Console.WriteLine($"Thick border width: {thickBorderWidth}");
                Console.WriteLine($"Dashed border width: {dashedBorderWidth}");

                // Guarda el libro de trabajo
                workbook.Save("GetCellBorderWidthDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [CellBorderType](../../../aspose.cells/cellbordertype/)
* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


