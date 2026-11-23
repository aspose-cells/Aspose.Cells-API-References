---
title: "Classe ReplaceOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ReplaceOptions. Représente les options de remplacement"
type: docs
url: /fr/net/aspose.cells/replaceoptions/
---
## ReplaceOptions class

Représente les options de remplacement.

```csharp
public class ReplaceOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ReplaceOptions](replaceoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CaseSensitive](../../aspose.cells/replaceoptions/casesensitive/) { get; set; } | Indique si la chaîne recherchée est sensible à la casse. |
| [FontSettings](../../aspose.cells/replaceoptions/fontsettings/) { get; set; } | Les paramètres richement formatés pour le texte remplacé. |
| [MatchEntireCellContents](../../aspose.cells/replaceoptions/matchentirecellcontents/) { get; set; } | Indique si le contenu complet des cellules doit correspondre |
| [RegexKey](../../aspose.cells/replaceoptions/regexkey/) { get; set; } | Indique si la clé recherchée est une expression régulière. Si true, la clé recherchée sera prise comme expression régulière. |
| [StyleFlags](../../aspose.cells/replaceoptions/styleflags/) { get; set; } | Obtient et définit les indicateurs d'application des paramètres de police. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReplaceOptionsDemo
    {
        public static void ReplaceOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            // Créer ReplaceOptions
            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false,
                RegexKey = false
            };

            // Remplacer "Hello" par "Hi" dans la feuille de calcul
            int replacedCount = workbook.Replace("Hello", "Hi", options);

            // Afficher le nombre de remplacements effectués
            Console.WriteLine($"Number of replacements made: {replacedCount}");

            // Enregistrez le classeur
            workbook.Save("ReplaceOptionsExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


