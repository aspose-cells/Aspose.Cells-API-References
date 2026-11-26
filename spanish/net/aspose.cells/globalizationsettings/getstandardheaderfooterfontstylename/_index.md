---
title: "GlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre del estilo de fuente estándar en inglés Regular Bold Italic para Encabezado/Pie de página según el nombre del estilo de fuente del locale dado"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/
---
## GlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Obtiene el nombre de estilo de fuente estándar en inglés (Regular, Bold, Italic) para Encabezado/Pie de página según el nombre de estilo de fuente dependiente de la configuración regional proporcionado.

```csharp
public virtual string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
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

    public class GlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear instancia de configuraciones de globalización personalizadas
            var globalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Demostrar llamada al método con tipo de parámetro (String)
                string localStyle = "CustomBold";
                string standardStyle = globalizationSettings.GetStandardHeaderFooterFontStyleName(localStyle);
                Console.WriteLine($"Converted font style: {localStyle} -> {standardStyle}");

                // Aplicar configuraciones de globalización al libro de trabajo
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Establecer encabezado con estilo de fuente personalizado que será convertido
                // Usar el método SetHeader con el parámetro de sección (0 = izquierda, 1 = centro, 2 = derecha)
                worksheet.PageSetup.SetHeader(1, "&\"Arial\"&\"CustomBold\"&12Header Text");

                // Guardar el libro de trabajo para mostrar el efecto
                workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
        }
    }

    // Implementación de configuración personalizada de globalización
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
        {
            // Convertir nombres de estilos de fuente personalizados a nombres estándar
            return localfontStyleName switch
            {
                "CustomBold" => "Bold",
                "CustomItalic" => "Italic",
                _ => base.GetStandardHeaderFooterFontStyleName(localfontStyleName)
            };
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


