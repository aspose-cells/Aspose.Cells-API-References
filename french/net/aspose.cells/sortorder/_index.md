---
title: "Enum SortOrder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.SortOrder enum. Représente l'ordre de tri pour la plage de données"
type: docs
url: /fr/net/aspose.cells/sortorder/
---
## SortOrder enumeration

Représente l'ordre de tri pour la plage de données.

```csharp
public enum SortOrder
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Ascending | `0` | Trie les données par ordre croissant |
| Descending | `1` | Trie les données par ordre décroissant |
| Natural | `2` | Conserve l'ordre original des données sans tri. S'applique uniquement à certains scénarios spéciaux tels que le tableau croisé dynamique. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSortOrderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            var workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à trier
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);
            
            // Créer un trieur de données
            var sorter = workbook.DataSorter;
            
            // Définir l'ordre de tri et les clés
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Définir la zone de tri
            var sortArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };
            
            // Effectuez le tri
            sorter.Sort(worksheet.Cells, sortArea);
            
            // Enregistrez le classeur
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


