---
title: "Cell.Replace"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Remplace le texte de la cellule avec des options"
type: docs
url: /fr/net/aspose.cells/cell/replace/
---
## Cell.Replace method

Remplace le texte de la cellule avec des options.

```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| placeHolder | String | Espace réservé de cellule |
| newValue | String | Valeur String à remplacer |
| options | ReplaceOptions | Les options de remplacement |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("hello world");
            worksheet.Cells["A3"].PutValue("HELLO WORLD");
            worksheet.Cells["B1"].PutValue("Replaced");

            // Créer des options de remplacement
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            options.MatchEntireCellContents = false;

            // Obtenir les paramètres de police de la cellule B1 pour les appliquer aux remplacements
            options.FontSettings = worksheet.Cells["B1"].GetCharacters();

            // Remplacer toutes les variantes de "hello" par "Hi" en utilisant les options
            foreach (Cell cell in worksheet.Cells)
            {
                cell.Replace("Hello", "Hi", options);
            }

            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


