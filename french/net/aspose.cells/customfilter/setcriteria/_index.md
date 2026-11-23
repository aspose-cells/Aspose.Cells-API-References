---
title: "CustomFilter.SetCriteria"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CustomFilter. Définit les critères du filtre"
type: docs
url: /fr/net/aspose.cells/customfilter/setcriteria/
---
## CustomFilter.SetCriteria method

Définit les critères du filtre.

```csharp
public void SetCriteria(FilterOperatorType filterOperator, object criteria)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filterOperator | FilterOperatorType | type d'opérateur de filtre |
| critères | Object | valeur des critères du filtre |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterMethodSetCriteriaWithFilterOperatorTObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);

            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;

            try
            {
                // Appliquez un filtre personnalisé pour obtenir une instance CustomFilter
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Obtenez le premier filtre personnalisé de la collection de filtres
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Définir les critères en utilisant la méthode SetCriteria
                customFilter.SetCriteria(FilterOperatorType.GreaterThan, 25);

                // Afficher les critères définis
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Enregistrez le classeur
                workbook.Save("SetCriteriaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


