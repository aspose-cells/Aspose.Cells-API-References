---
title: "Worksheet.ClearComments"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Supprime tous les commentaires dans la feuille de calcul du concepteur"
type: docs
url: /fr/net/aspose.cells/worksheet/clearcomments/
---
## Worksheet.ClearComments method

Efface tous les commentaires dans la feuille de calcul du concepteur.

```csharp
public void ClearComments()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des commentaires d'exemple aux cellules en utilisant les références de cellules
            int comment1 = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1].Note = "This is comment 1";
            
            int comment2 = worksheet.Comments.Add("B3");
            worksheet.Comments[comment2].Note = "This is comment 2";
            
            int comment3 = worksheet.Comments.Add("C5");
            worksheet.Comments[comment3].Note = "This is comment 3";

            // Afficher le nombre de commentaires avant la suppression
            Console.WriteLine($"Comments count before ClearComments(): {worksheet.Comments.Count}");

            // Supprimer tous les commentaires de la feuille de calcul
            worksheet.ClearComments();

            // Afficher le nombre de commentaires après la suppression
            Console.WriteLine($"Comments count after ClearComments(): {worksheet.Comments.Count}");

            // Enregistrez le classeur
            workbook.Save("ClearCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


