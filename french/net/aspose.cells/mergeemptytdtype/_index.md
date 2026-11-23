---
title: "Enum MergeEmptyTdType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.MergeEmptyTdType. Représente le type de fusion pour un élément TD vide lors de l'exportation d'un fichier vers HTML"
type: docs
url: /fr/net/aspose.cells/mergeemptytdtype/
---
## MergeEmptyTdType enumeration

Représente le type de fusion pour un élément TD vide lors de l'exportation d'un fichier en HTML.

```csharp
public enum MergeEmptyTdType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | Affichage similaire à MS Excel. |
| None | `1` | Les éléments TD vides ne seront pas fusionnés lors de l'exportation du fichier vers HTML. Cela générera un fichier HTML nettement plus volumineux. |
| MergeForcely | `2` | Fusion forcée des éléments TD vides lors de l'exportation du fichier vers HTML. La taille du fichier HTML sera considérablement réduite après avoir défini la valeur sur true. Si vous souhaitez importer le fichier HTML dans Excel ou exporter des lignes de grille parfaites lors de l'enregistrement du fichier en HTML, veuillez conserver la valeur par défaut. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MergeEmptyTdTypeDemo
    {
        public static void MergeEmptyTdTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Data1");
            worksheet.Cells["B1"].PutValue("Data2");
            worksheet.Cells["C1"].PutValue("Data3");

            // Créez HtmlSaveOptions et définissez la propriété MergeEmptyTdType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.MergeForcely;

            // Enregistrer le classeur au format HTML
            workbook.Save("MergeEmptyTdTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with MergeEmptyTdType.MergeForcely option.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


