---
title: "WorksheetCollection.SortNames"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WorksheetCollection méthode. Trie les noms définis"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/sortnames/
---
## WorksheetCollection.SortNames method

Trie les noms définis.

```csharp
public void SortNames()
```

### Remarques

Si vous créez un grand nombre de plages nommées dans le fichier Excel, veuillez appeler cette méthode après la création de toutes les plages nommées et avant l'enregistrement

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSortNamesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter quelques plages nommées
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test1");
            worksheet.Cells.CreateRange("A1").Name = "Range2";
            worksheet.Cells["B1"].PutValue("Test2");
            worksheet.Cells.CreateRange("B1").Name = "Range1";
            
            // Afficher les noms avant le tri
            Console.WriteLine("Before sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Trier les noms
            workbook.Worksheets.SortNames();
            
            // Afficher les noms après le tri
            Console.WriteLine("\nAfter sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


