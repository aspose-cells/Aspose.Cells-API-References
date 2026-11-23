---
title: "ListObject.HasAutoFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListObject. Indique si le filtre automatique est appliqué à ce tableau"
type: docs
url: /fr/net/aspose.cells.tables/listobject/hasautofilter/
---
## ListObject.HasAutoFilter property

Indique si le filtre automatique est appliqué à ce tableau.

```csharp
public bool HasAutoFilter { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Tables;

    public class ListObjectPropertyHasAutoFilterDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir le tableau avec des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Charlie");
            worksheet.Cells["B4"].PutValue(78);

            try
            {
                // Ajouter un ListObject (tableau) couvrant la plage de données
                int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[tableIndex];

                // S'assurer que le tableau est redimensionné pour inclure toutes les lignes
                listObject.Resize(0, 0, 4, 2, true);

                // Lire et afficher la valeur de la propriété HasAutoFilter
                bool hasFilter = listObject.HasAutoFilter;
                Console.WriteLine("HasAutoFilter: " + hasFilter);

                // L'objet AutoFilter peut être accédé via la propriété AutoFilter
                // Démontrer qu'il n'est pas nul lorsque HasAutoFilter est vrai
                if (hasFilter && listObject.AutoFilter != null)
                {
                    // Appliquer un filtre simple sur la colonne "Score" (index 1) pour afficher les lignes avec Score >= 80
                    listObject.AutoFilter.Filter(1, ">=80");

                    Console.WriteLine("Filtered rows (Score >= 80):");
                    for (int row = 1; row <= 4; row++)
                    {
                        // Utiliser Cells.Rows pour vérifier si la ligne est masquée
                        if (!worksheet.Cells.Rows[row].IsHidden)
                        {
                            Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                        }
                    }

                    // Effacer le filtre
                    listObject.AutoFilter.RemoveFilter(1);
                }

                // Enregistrer le classeur (facultatif)
                workbook.Save("HasAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


