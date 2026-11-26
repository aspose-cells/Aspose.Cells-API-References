---
title: "CustomRenderSettings.CustomRenderSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor CustomRenderSettings. Ctor"
type: docs
url: /es/net/aspose.cells.rendering/customrendersettings/customrendersettings/
---
## CustomRenderSettings constructor

Ctor.

```csharp
public CustomRenderSettings()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";

            try
            {
                // Crea una instancia de CustomRenderSettings usando el constructor
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Muestra la confirmación de la llamada exitosa al constructor
                Console.WriteLine("CustomRenderSettings instance created successfully using #ctor");

                // Demuestra que la instancia funciona llamando a un método
                float borderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                Console.WriteLine($"Default thin border width: {borderWidth}");

                // Guarda el libro de trabajo
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomRenderSettings: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


