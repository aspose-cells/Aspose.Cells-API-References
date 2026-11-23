---
title: "Enum FilterCategory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.FilterCategory. Représente la catégorie du filtre"
type: docs
url: /fr/net/aspose.cells/filtercategory/
---
## FilterCategory enumeration

Représente la catégorie du filtre.

```csharp
public enum FilterCategory
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Pas de filtre. |
| Label | `1` | Filtre de légende. |
| NumberValue | `2` | Filtre de valeur numérique. |
| Date | `3` | Filtre de valeur de date. |
| Top10 | `4` | Filtre de valeur Top10. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CellsClassFilterCategoryDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            CreateSampleData(worksheet);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:C7", "H5");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configurer les champs de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            
            // Configurer le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Ajouter un filtre d'étiquette aux filtres du tableau croisé dynamique
            PivotFilter filter = pivotTable.PivotFilters.AddLabelFilter(0, PivotFilterType.CaptionEqual, "East", null);
            
            // Démontrer l'utilisation de FilterCategory
            Console.WriteLine("Filter Category: " + filter.FilterCategory);
            
            // Afficher toutes les catégories de filtres dans le tableau croisé dynamique
            foreach (PivotFilter pivotFilter in pivotTable.PivotFilters)
            {
                Console.WriteLine($"Filter Type: {pivotFilter.FilterType}, Category: {pivotFilter.FilterCategory}");
            }

            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrer le résultat
            workbook.Save("FilterCategoryDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Définir les en-têtes des données d'exemple
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";

            // Ajouter des lignes de données d'exemple
            object[,] data = new object[,]
            {
                {"East", "Apples", 5000},
                {"West", "Oranges", 3000},
                {"East", "Bananas", 4000},
                {"North", "Apples", 6000},
                {"South", "Oranges", 2000},
                {"East", "Bananas", 4500},
                {"West", "Apples", 5500}
            };

            int rowCount = data.GetLength(0);
            int colCount = data.GetLength(1);

            for (int i = 0; i < rowCount; i++)
            {
                for (int j = 0; j < colCount; j++)
                {
                    worksheet.Cells[i + 2, j].Value = data[i, j];
                }
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


