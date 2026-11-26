---
title: "PaginatedSaveOptions.CustomRenderSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Obtiene o establece configuraciones personalizadas durante el renderizado"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/customrendersettings/
---
## PaginatedSaveOptions.CustomRenderSettings property

Obtiene o establece configuraciones personalizadas durante el renderizado.

```csharp
public CustomRenderSettings CustomRenderSettings { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "This demonstrates CustomRenderSettings property";

            try
            {
                // Cree PdfSaveOptions que hereda de PaginatedSaveOptions
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Obtenga el valor actual de CustomRenderSettings
                CustomRenderSettings currentSettings = saveOptions.CustomRenderSettings;
                Console.WriteLine("Current CustomRenderSettings: " +
                    (currentSettings == null ? "null" : "CustomRenderSettings instance"));

                // Cree y establezca nuevas CustomRenderSettings
                CustomRenderSettings newSettings = new CustomRenderSettings();
                saveOptions.CustomRenderSettings = newSettings;

                // Verifique que se hayan aplicado las nuevas configuraciones
                Console.WriteLine("New CustomRenderSettings set: " +
                    (saveOptions.CustomRenderSettings == newSettings ? "Success" : "Failed"));

                // Guarde el libro de trabajo con las configuraciones de renderizado personalizadas
                workbook.Save("CustomRenderSettingsDemo.pdf", saveOptions);
                Console.WriteLine("Workbook saved with CustomRenderSettings");
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

* class [CustomRenderSettings](../../../aspose.cells.rendering/customrendersettings/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


