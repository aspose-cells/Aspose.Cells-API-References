---
title: "AdvancedFilter.CriteriaRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AdvancedFilter. Obtient la plage de critères de ce filtre avancé"
type: docs
url: /fr/net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

Obtient la plage de critères de ce filtre avancé.

```csharp
public string CriteriaRange { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Remplissez les données d'exemple pour la plage de la liste
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Food");
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue("Transport");
            sheet.Cells["B3"].PutValue(80);
            sheet.Cells["A4"].PutValue("Food");
            sheet.Cells["B4"].PutValue(150);

            // Remplir les critères d'exemple (le filtre les utilisera lorsqu'il sera appliqué)
            sheet.Cells["D1"].PutValue("Category");
            sheet.Cells["D2"].PutValue("Food");

            try
            {
                // Obtenir l'objet AdvancedFilter pour la feuille de calcul
                AdvancedFilter filter = sheet.GetAdvancedFilter();

                // Les propriétés ListRange, CriteriaRange et CopyToRange sont en lecture seule.
                // Afficher les plages déterminées automatiquement.
                Console.WriteLine("List Range:    " + filter.ListRange);
                Console.WriteLine("Criteria Range:" + filter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + filter.CopyToRange);

                // Enregistrer le classeur (optionnel, juste pour montrer que le fichier peut être créé)
                workbook.Save("AdvancedFilterCriteriaRangeDemo.xlsx");
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

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


