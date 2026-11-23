---
title: "FontConfigs.SetFontFolder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FontConfigs. Définit le dossier des polices"
type: docs
url: /fr/net/aspose.cells/fontconfigs/setfontfolder/
---
## FontConfigs.SetFontFolder method

Définit le dossier des polices

```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolder | String | Le dossier qui contient les polices TrueType. |
| recursive | Boolean | Détermine s'il faut ou non analyser les sous-dossiers. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Initialiser un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter du texte à la cellule A1
            worksheet.Cells["A1"].PutValue("Sample Text with Custom Font");
            
            // Définir le dossier de polices personnalisé et spécifier s'il faut inclure les sous‑dossiers
            FontConfigs.SetFontFolder("Fonts", true);
            
            // Appliquer un style de police qui pourrait utiliser des polices du dossier personnalisé
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "CustomFont"; // Assuming "CustomFont" exists in the Fonts folder
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Enregistrez le classeur au format PDF
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Voir aussi

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


