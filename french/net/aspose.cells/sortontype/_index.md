---
title: "Énum SortOnType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énum Aspose.Cells.SortOnType. Type de valeur triée"
type: docs
url: /fr/net/aspose.cells/sortontype/
---
## SortOnType enumeration

Type de valeur triée.

```csharp
public enum SortOnType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Value | `0` | Trie par la valeur des cellules. |
| CellColor | `1` | Trie par la couleur des cellules. |
| FontColor | `2` | Trie par la couleur de police des cellules. |
| Icon | `3` | Trie par l'icône conditionnelle. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SortOnTypeDemo
    {
        public static void SortOnTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(95);
            worksheet.Cells["B4"].PutValue(75);

            // Applique le filtre automatique à la plage
            worksheet.AutoFilter.Range = "A1:B4";

            // Obtenir le filtre automatique
            AutoFilter autoFilter = worksheet.AutoFilter;

            // Obtenir le trieur de données
            DataSorter sorter = autoFilter.Sorter;

            // Définir la première clé pour trier par les valeurs de la deuxième colonne (Score)
            sorter.AddKey(1, SortOnType.Value, SortOrder.Descending, null);

            // Trier les données dans la plage
            sorter.Sort(worksheet.Cells, 1, 0, 3, 1);

            // Enregistrez le classeur
            workbook.Save("SortOnTypeExample.xlsx");

            // Afficher les résultats
            Console.WriteLine("Data sorted by Score in descending order.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


