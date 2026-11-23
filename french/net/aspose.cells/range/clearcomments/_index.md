---
title: "Range.ClearComments"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Supprime les commentaires de cette plage"
type: docs
url: /fr/net/aspose.cells/range/clearcomments/
---
## Range.ClearComments method

Efface les commentaires de cette plage.

```csharp
public void ClearComments()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données et des commentaires aux cellules
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A1"].PutValue("This is a comment on A1", true, false);
            worksheet.Cells["B2"].Value = "More Data";
            worksheet.Cells["B2"].PutValue("This is a comment on B2", true, false);

            try
            {
                // Créer une plage qui inclut des cellules avec des commentaires
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Supprimer les commentaires de la plage
                range.ClearComments();

                Console.WriteLine("Comments cleared successfully from range A1:B2");
                Console.WriteLine($"Cell A1 value after clearing: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell B2 value after clearing: {worksheet.Cells["B2"].Value}");

                // Enregistrez le classeur
                workbook.Save("ClearCommentsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearComments: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


