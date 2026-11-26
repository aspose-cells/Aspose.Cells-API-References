---
title: "DefaultStyleSettings.BuiltInPreference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad DefaultStyleSettings. Indica si la propiedad para el formato numérico es preferible cuando el estilo define tanto número incorporado como patrón personalizado. El valor predeterminado es false, lo que significa que por defecto se utilizará el patrón personalizado para formatear valores siempre que no esté vacío para un estilo"
type: docs
url: /es/net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

Indica si la propiedad de formato numérico es preferible cuando el estilo define tanto un número incorporado como un patrón personalizado. El valor predeterminado es false, lo que significa que, por defecto, se utilizará el patrón personalizado para formatear valores siempre que no esté vacío para un estilo.

```csharp
public bool BuiltInPreference { get; set; }
```

### Observaciones

Al cargar un libro de trabajo desde un archivo de plantilla existente, puede que tanto el número incorporado como el patrón personalizado estén definidos para un estilo. Esta propiedad determina si debemos usar el número incorporado o el patrón personalizado al formatear valores con el estilo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyBuiltInPreferenceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración de estilo predeterminado
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Demostrar la propiedad BuiltInPreference
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12;

            // Aplicar a la hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Guarda el libro de trabajo
            workbook.Save("BuiltInPreferenceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


