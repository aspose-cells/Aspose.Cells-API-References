---
title: "Classe FontConfigs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FontConfigs. Spécifie les paramètres de police"
type: docs
url: /fr/net/aspose.cells/fontconfigs/
---
## FontConfigs class

Spécifie les paramètres de police

```csharp
public class FontConfigs
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FontConfigs](fontconfigs/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| static [DefaultFontName](../../aspose.cells/fontconfigs/defaultfontname/) { get; set; } | Obtient ou définit le nom de police par défaut. |
| static [PreferSystemFontSubstitutes](../../aspose.cells/fontconfigs/prefersystemfontsubstitutes/) { get; set; } | Indique s'il faut d'abord utiliser les substituts de police du système ou non lorsqu'une police n'est pas disponible et que le substitut de cette police n'est pas défini. Par exemple, sous Ubuntu, la police "Arial" est généralement substituée par "Liberation Sans". La valeur par défaut est false. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [GetFontFileDataInfo](../../aspose.cells/fontconfigs/getfontfiledatainfo/)(string, bool, bool, bool) | Obtenir les informations de données du fichier de police. |
| static [GetFontSources](../../aspose.cells/fontconfigs/getfontsources/)() | Obtient une copie du tableau contenant la liste des sources |
| static [GetFontSubstitutes](../../aspose.cells/fontconfigs/getfontsubstitutes/)(string) | Renvoie un tableau contenant les noms de substituts de police à utiliser si la police d'origine n'est pas présente. |
| static [IsFontAvailable](../../aspose.cells/fontconfigs/isfontavailable/)(string) | Indique si la police est disponible. |
| static [SetFontFolder](../../aspose.cells/fontconfigs/setfontfolder/)(string, bool) | Définit le dossier des polices |
| static [SetFontFolders](../../aspose.cells/fontconfigs/setfontfolders/)(string[], bool) | Définit le dossier des polices |
| static [SetFontSources](../../aspose.cells/fontconfigs/setfontsources/)(FontSourceBase[]) | Définit les sources de police. |
| static [SetFontSubstitutes](../../aspose.cells/fontconfigs/setfontsubstitutes/)(string, string[]) | Noms de substituts de police pour le nom de police d'origine donné. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontConfigsDemo
    {
        public static void Run()
        {
            // Définir le dossier de police personnalisé
            string fontFolder = @"C:\MyFonts\";
            FontConfigs.SetFontFolder(fontFolder, true);

            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir le texte d'exemple avec différentes polices
            worksheet.Cells["A1"].PutValue("Text with default font");
            worksheet.Cells["A2"].PutValue("Text with custom font");
            
            // Appliquer le style de police personnalisé
            Style style = workbook.CreateStyle();
            style.Font.Name = "MyCustomFont"; // This font should exist in the custom font folder
            worksheet.Cells["A2"].SetStyle(style);

            // Enregistrer en HTML pour démontrer le rendu des polices
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportImagesAsBase64 = true,
                PresentationPreference = true
            };
            
            workbook.Save("output.html", options);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


