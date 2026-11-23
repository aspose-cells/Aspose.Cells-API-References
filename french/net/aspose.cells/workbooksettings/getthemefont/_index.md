---
title: "WorkbookSettings.GetThemeFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode WorkbookSettings. Obtient le nom de la police de thème par défaut"
type: docs
url: /fr/net/aspose.cells/workbooksettings/getthemefont/
---
## WorkbookSettings.GetThemeFont method

Obtient le nom de police du thème par défaut.

```csharp
public string GetThemeFont(FontSchemeType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | FontSchemeType | Le type de schéma de la police. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodGetThemeFontWithFontSchemeTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenir la police de thème par défaut pour le type de schéma mineur
            string minorFont = workbook.Settings.GetThemeFont(FontSchemeType.Minor);
            Console.WriteLine("Minor theme font: " + minorFont);
            
            // Obtenir la police de thème par défaut pour le type de schéma majeur
            string majorFont = workbook.Settings.GetThemeFont(FontSchemeType.Major);
            Console.WriteLine("Major theme font: " + majorFont);
            
            // Enregistrez le classeur
            workbook.Save("ThemeFontExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FontSchemeType](../../fontschemetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


