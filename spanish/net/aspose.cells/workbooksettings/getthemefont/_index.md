---
title: "WorkbookSettings.GetThemeFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorkbookSettings. Obtiene el nombre de la fuente de tema predeterminada"
type: docs
url: /es/net/aspose.cells/workbooksettings/getthemefont/
---
## WorkbookSettings.GetThemeFont method

Obtiene el nombre de fuente predeterminado del tema.

```csharp
public string GetThemeFont(FontSchemeType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | FontSchemeType | El tipo de esquema de la fuente. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodGetThemeFontWithFontSchemeTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener la fuente de tema predeterminada para el tipo de esquema menor
            string minorFont = workbook.Settings.GetThemeFont(FontSchemeType.Minor);
            Console.WriteLine("Minor theme font: " + minorFont);
            
            // Obtener la fuente de tema predeterminada para el tipo de esquema mayor
            string majorFont = workbook.Settings.GetThemeFont(FontSchemeType.Major);
            Console.WriteLine("Major theme font: " + majorFont);
            
            // Guarda el libro de trabajo
            workbook.Save("ThemeFontExample.xlsx");
        }
    }
}
```

### Ver también

* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


