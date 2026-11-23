---
title: "AdvancedFilter.CopyToRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AdvancedFilter. Obtient la plage où copier le résultat de ce filtre avancé"
type: docs
url: /fr/net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

Obtient la plage où copier le résultat de ce filtre avancé.

```csharp
public string CopyToRange { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCopyToRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Obtenir la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(1.2);

            // Ajouter la plage de critères
            worksheet.Cells["D1"].PutValue("Product");
            worksheet.Cells["D2"].PutValue("Apple");

            try
            {
                // Obtenez l'instance AdvancedFilter de la feuille de calcul
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Afficher la valeur de la propriété CopyToRange
                Console.WriteLine("CopyToRange value: " + advancedFilter.CopyToRange);

                // Enregistrez le classeur
                workbook.Save("CopyToRangeDemo.xlsx");
                Console.WriteLine("CopyToRange demonstration completed successfully.");
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


