---
title: "FilterColumn.Top10Filter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FilterColumn. Obtient Top10Filter pour filtrer les données selon leur rang"
type: docs
url: /fr/net/aspose.cells/filtercolumn/top10filter/
---
## FilterColumn.Top10Filter property

Obtient `Top10Filter` pour filtrer les données selon leur rang.

```csharp
public Top10Filter Top10Filter { get; }
```

### Remarques

Avant d'utiliser cette propriété, veuillez vous assurer que [`FilterType`](../filtertype/) est Top10, sinon null sera renvoyé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyTop10FilterDemo
    {
        public static void Run()
        {
            try
            {
                // Créez un nouveau classeur et obtenez la première feuille de calcul
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Remplir des données d'exemple
                sheet.Cells["A1"].PutValue("Values");
                sheet.Cells["A2"].PutValue(10);
                sheet.Cells["A3"].PutValue(20);
                sheet.Cells["A4"].PutValue(30);
                sheet.Cells["A5"].PutValue(40);

                // Appliquer un AutoFilter à la plage de données
                sheet.AutoFilter.Range = "A1:A5";

                // Obtenir la première colonne de filtre (indice de colonne 0)
                FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

                // Afficher l'objet Filter actuel (peut être null)
                Console.WriteLine("Current Filter object type: " +
                    (filterColumn.Filter != null ? filterColumn.Filter.GetType().FullName : "null"));

                // Vérifier si le filtre appliqué est un Top10Filter
                if (filterColumn.Filter != null && filterColumn.Filter.GetType().Name == "Top10Filter")
                {
                    Console.WriteLine("The filter column contains a Top10Filter.");
                }
                else
                {
                    Console.WriteLine("No Top10Filter is applied to this column.");
                }

                // Enregistrer le classeur (facultatif)
                workbook.Save("Top10FilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Top10Filter](../../top10filter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


