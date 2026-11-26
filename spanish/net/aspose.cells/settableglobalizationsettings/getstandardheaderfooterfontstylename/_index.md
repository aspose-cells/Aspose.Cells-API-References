---
title: "SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre de estilo de fuente estándar en inglés Regular Bold Italic para Header/Footer según el nombre de estilo de fuente de la configuración regional proporcionado"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Obtiene el nombre de estilo de fuente estándar en inglés (Regular, Bold, Italic) para Encabezado/Pie de página según el nombre de estilo de fuente dependiente de la configuración regional proporcionado.

```csharp
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| localfontStyleName | String | Nombre de estilo de fuente de la configuración regional para Header/Footer. |

### Valor de retorno

Nombre de estilo de fuente estándar en inglés (Regular, Bold, Italic)

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Establecer un mapeo de nombre de estilo de fuente estándar para encabezado/pie de página
            settings.SetStandardHeaderFooterFontStyleName("MyLocalFontStyle", "Arial");

            // Aplicar la configuración al workbook
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Llame al método GetStandardHeaderFooterFontStyleName con un nombre de estilo de fuente local
                string standardFontStyle = settings.GetStandardHeaderFooterFontStyleName("MyLocalFontStyle");
                
                // Mostrar el resultado
                Console.WriteLine($"Standard font style name for 'MyLocalFontStyle': {standardFontStyle}");

                // Cree un encabezado con el nombre de estilo de fuente local
                worksheet.PageSetup.SetHeader(1, "&\"MyLocalFontStyle\"&12Test Header");

                // Muestre el efecto en la hoja de cálculo
                Console.WriteLine("Header set with local font style name 'MyLocalFontStyle'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


