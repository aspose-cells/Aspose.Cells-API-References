---
title: "NameCollection.Sort"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode NameCollection. Trie les noms définis"
type: docs
url: /fr/net/aspose.cells/namecollection/sort/
---
## NameCollection.Sort method

Trie les noms définis.

```csharp
public void Sort()
```

### Remarques

Si vous créez un grand nombre de plages nommées dans le fichier Excel, veuillez appeler cette méthode après la création de toutes les plages nommées et avant l'enregistrement

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodSortDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenez le NameCollection du classeur
            NameCollection names = workbook.Worksheets.Names;
            
            // Ajoutez quelques plages nommées pour démontrer le tri
            names.Add("RangeC");
            names.Add("RangeA");
            names.Add("RangeB");
            
            try
            {
                // Afficher les noms avant le tri
                Console.WriteLine("Names before sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
                
                // Appelez la méthode Sort
                names.Sort();
                
                // Afficher les noms après le tri
                Console.WriteLine("\nNames after sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Sort method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("NameCollectionSortDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


