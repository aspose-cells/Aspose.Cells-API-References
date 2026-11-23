---
title: "NameCollection.RemoveDuplicateNames"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode NameCollection. Supprimer les noms définis en double"
type: docs
url: /fr/net/aspose.cells/namecollection/removeduplicatenames/
---
## NameCollection.RemoveDuplicateNames method

Supprimer les noms définis en double

```csharp
public void RemoveDuplicateNames()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveDuplicateNamesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter quelques plages nommées avec des noms en double
            worksheet.Cells["A1"].PutValue("Test Value 1");
            worksheet.Cells["B1"].PutValue("Test Value 2");
            
            // Créer des plages nommées en double en utilisant la signature correcte de la méthode Add
            int index1 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$B$1";
            
            // Afficher le nombre avant de supprimer les doublons
            Console.WriteLine($"Named ranges count before removal: {workbook.Worksheets.Names.Count}");
            
            // Supprimer les noms en double
            workbook.Worksheets.Names.RemoveDuplicateNames();
            
            // Afficher le nombre après la suppression des doublons
            Console.WriteLine($"Named ranges count after removal: {workbook.Worksheets.Names.Count}");
        }
    }
}
```

### Voir aussi

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


