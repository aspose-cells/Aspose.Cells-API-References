---
title: "ImageOrPrintOptions.CustomRenderSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece configuraciones personalizadas durante el renderizado"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/customrendersettings/
---
## ImageOrPrintOptions.CustomRenderSettings property

Obtiene o establece configuraciones personalizadas durante el renderizado.

```csharp
public CustomRenderSettings CustomRenderSettings { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class ImageOrPrintOptionsPropertyCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con algunos datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo for CustomRenderSettings");
            sheet.Cells["B2"].PutValue(12345);
            sheet.Cells["C3"].PutValue(DateTime.Now);

            try
            {
                // Inicializar ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Acceder a la propiedad CustomRenderSettings (solo lectura) y mostrar su estado actual
                var customRenderSettings = options.CustomRenderSettings;
                Console.WriteLine("CustomRenderSettings instance: " +
                                  (customRenderSettings != null ? customRenderSettings.GetType().FullName : "null"));

                // Opcionalmente demostrar que las opciones aún funcionan para el renderizado
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                SheetRender renderer = new SheetRender(sheet, options);
                renderer.ToImage(0, "CustomRenderSettingsDemo.png");

                Console.WriteLine("Image rendered successfully.");
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

* class [CustomRenderSettings](../../customrendersettings/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


