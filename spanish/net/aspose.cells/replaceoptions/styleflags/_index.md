---
title: "ReplaceOptions.StyleFlags"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReplaceOptions. Obtiene y establece banderas de aplicación de configuraciones de fuente"
type: docs
url: /es/net/aspose.cells/replaceoptions/styleflags/
---
## ReplaceOptions.StyleFlags property

Obtiene y establece banderas de aplicación de configuraciones de fuente.

```csharp
public StyleFlag[] StyleFlags { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyStyleFlagsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar texto de muestra a la celda
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("test text");

            // Crear opciones de reemplazo
            ReplaceOptions options = new ReplaceOptions();
            options.MatchEntireCellContents = false;
            options.CaseSensitive = false;

            // Crear configuración de fuente y bandera de estilo
            string replacementText = "new text";
            FontSetting setting = new FontSetting(0, replacementText.Length, workbook.Worksheets);
            StyleFlag styleFlag = new StyleFlag();
            
            // Configurar fuente y estilo
            setting.Font.Color = Color.Red;
            setting.Font.Underline = FontUnderlineType.Single;
            styleFlag.FontColor = true;
            styleFlag.FontUnderline = true;

            // Aplicar configuraciones a las opciones
            options.FontSettings = new FontSetting[] { setting };
            options.StyleFlags = new StyleFlag[] { styleFlag };

            // Realizar reemplazo
            workbook.Replace("test", replacementText, options);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [StyleFlag](../../styleflag/)
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


