---
title: "Clase DefaultStyleSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DefaultStyleSettings. Configuraciones para los valores predeterminados de las propiedades de estilo del libro de trabajo"
type: docs
url: /es/net/aspose.cells/defaultstylesettings/
---
## DefaultStyleSettings class

Configuraciones para los valores predeterminados de las propiedades de estilo del libro de trabajo.

```csharp
public class DefaultStyleSettings
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BuiltInPreference](../../aspose.cells/defaultstylesettings/builtinpreference/) { get; set; } | Indica si la propiedad de formato numérico es preferible cuando el estilo define tanto un número incorporado como un patrón personalizado. El valor predeterminado es false, lo que significa que, por defecto, se utilizará el patrón personalizado para formatear valores siempre que no esté vacío para un estilo. |
| [FontName](../../aspose.cells/defaultstylesettings/fontname/) { get; set; } | Obtiene/Establece el nombre de fuente predeterminado para el libro de trabajo |
| [FontSize](../../aspose.cells/defaultstylesettings/fontsize/) { get; set; } | Obtiene/Establece el tamaño de fuente estándar predeterminado para el libro de trabajo. |
| [HorizontalAlignment](../../aspose.cells/defaultstylesettings/horizontalalignment/) { get; set; } | Obtiene/Establece el valor predeterminado para la alineación horizontal |
| [VerticalAlignment](../../aspose.cells/defaultstylesettings/verticalalignment/) { get; set; } | Obtiene/Establece el valor predeterminado para la alineación vertical |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultStyleSettingsDemo
    {
        public static void DefaultStyleSettingsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la configuración de estilo predeterminada del libro de trabajo
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Estableciendo propiedades
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12.0;
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
            defaultStyleSettings.VerticalAlignment = TextAlignmentType.Center;

            // Aplique la configuración de estilo predeterminada a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            // Guarda el libro de trabajo
            workbook.Save("DefaultStyleSettingsExample.xlsx");
            workbook.Save("DefaultStyleSettingsExample.pdf");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


