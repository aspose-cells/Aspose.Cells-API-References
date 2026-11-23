---
title: "ListObject.Filter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListObject. Filtrer le tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/filter/
---
## ListObject.Filter method

Filtrer le tableau.

```csharp
[Obsolete("Use set ListObject.HasAutoFilter property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter Filter()
```

### Remarques

NOTE: Ce membre est maintenant obsolète. Au lieu de cela, veuillez définir la propriété ListObject.HasAutoFilter./// Cette propriété sera supprimée 12 mois plus tard à compter d'octobre 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectMethodFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple pour l'objet de liste
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Smartphone");
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Monitor");
            worksheet.Cells["B4"].PutValue(250);

            try
            {
                // Créer un objet de liste à partir d'une plage de données en utilisant ListObjects.Add avec les paramètres corrects
                int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[listObjectIndex];
                
                // Obtenir AutoFilter via la méthode Filter
                AutoFilter autoFilter = listObject.Filter();

                // Appliquer un filtre sur la colonne Prix (index 1) pour afficher les éléments >= 800
                autoFilter.Custom(1, FilterOperatorType.GreaterOrEqual, 800);

                Console.WriteLine("Filter applied successfully. Showing items with Price >= 800.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Filter method: {ex.Message}");
            }

            workbook.Save("ListObjectMethodFilterDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


