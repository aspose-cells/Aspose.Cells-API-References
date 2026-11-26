---
title: "ReplaceOptions.FontSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReplaceOptions. La configuración de formato enriquecido para el texto reemplazado"
type: docs
url: /es/net/aspose.cells/replaceoptions/fontsettings/
---
## ReplaceOptions.FontSettings property

La configuración de formato enriquecido para el texto reemplazado.

```csharp
public FontSetting[] FontSettings { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyFontSettingsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer texto de ejemplo en la celda A1
            worksheet.Cells["A1"].Value = "Sample text for replacement";
            
            // Crear opciones de reemplazo con configuración de fuente
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            
            // Crear configuración de fuente para el texto de reemplazo
            FontSetting fontSetting = new FontSetting(0, 8, workbook.Worksheets);
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Color = Color.Blue;
            
            // Aplicar configuración de fuente a las opciones de reemplazo
            options.FontSettings = new FontSetting[] { fontSetting };
            
            // Realizar el reemplazo
            workbook.Replace("text", "REPLACED", options);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../../fontsetting/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


