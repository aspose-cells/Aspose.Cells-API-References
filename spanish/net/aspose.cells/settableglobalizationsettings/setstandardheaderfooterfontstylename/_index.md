---
title: "SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre de función dependiente de la configuración regional según el nombre de función estándar proporcionado"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/setstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.SetStandardHeaderFooterFontStyleName method

Establece el nombre de función dependiente de la configuración regional según el nombre de función estándar dado.

```csharp
public void SetStandardHeaderFooterFontStyleName(string localfontStyleName, string standardName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| localfontStyleName | String | Nombre de estilo de fuente de la configuración regional para Header/Footer. |
| standardName | String | Nombre de función estándar (configuración regional en-US). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardHeaderFooterFontStyleNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree opciones de configuración de página para la hoja de cálculo
            PageSetup pageSetup = worksheet.PageSetup;

            // Establezca un encabezado con algún texto
            pageSetup.SetHeader(0, "&\"Arial\"&12This is a header");

            // Cree una instancia de configuración de globalización
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Llame al método SetStandardHeaderFooterFontStyleName
                globalizationSettings.SetStandardHeaderFooterFontStyleName("Arial", "Times New Roman");

                // Aplicar la configuración de globalización al libro de trabajo
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                Console.WriteLine("SetStandardHeaderFooterFontStyleName method executed successfully with parameters (\"Arial\", \"Times New Roman\")");

                // El efecto será visible cuando el documento se renderice o imprima
                // El estilo de fuente "Arial" en encabezados/pies de página será tratado como "Times New Roman"
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("MethodSetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


