---
title: "PivotFilter.AutoFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFilter. Obtient l'autofiltre du filtre pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/autofilter/
---
## PivotFilter.AutoFilter property

Obtient l'autofiltre du filtre pivot.

```csharp
[Obsolete("Use FilterLabel, FilterValue,FilterDate or FilterTop10 method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter AutoFilter { get; }
```

### Remarques

NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser les méthodes FilterLabel, FilterValue, FilterDate ou FilterTop10. Cette méthode sera supprimée 12 mois plus tard à compter de novembre 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une feuille de calcul et la remplir avec des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Ajouter des champs de ligne et de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Actualiser les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Ajoutez un filtre au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.PageFields[0];

            // Créer et ajouter un filtre
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];

            try
            {
                // Afficher la valeur de la propriété AutoFilter (lecture seule)
                Console.WriteLine("AutoFilter Range: " + filter.AutoFilter.Range);
                Console.WriteLine("AutoFilter ShowFilterButton: " + filter.AutoFilter.ShowFilterButton);

                // Démontrer l'accès aux propriétés AutoFilter
                Console.WriteLine("AutoFilter has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("PivotFilterAutoFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


