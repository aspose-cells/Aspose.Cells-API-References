---
title: "WorkbookSettings.GetThemeFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorkbookSettings. Ottiene il nome del carattere predefinito del tema"
type: docs
url: /it/net/aspose.cells/workbooksettings/getthemefont/
---
## WorkbookSettings.GetThemeFont method

Ottiene il nome del carattere predefinito del tema.

```csharp
public string GetThemeFont(FontSchemeType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | FontSchemeType | Il tipo di schema del carattere. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodGetThemeFontWithFontSchemeTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni il carattere predefinito del tema per il tipo di schema minore
            string minorFont = workbook.Settings.GetThemeFont(FontSchemeType.Minor);
            Console.WriteLine("Minor theme font: " + minorFont);
            
            // Ottieni il carattere predefinito del tema per il tipo di schema maggiore
            string majorFont = workbook.Settings.GetThemeFont(FontSchemeType.Major);
            Console.WriteLine("Major theme font: " + majorFont);
            
            // Salva la cartella di lavoro
            workbook.Save("ThemeFontExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


