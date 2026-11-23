---
title: "NameCollection.Remove"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode NameCollection. Supprimer un tableau de noms"
type: docs
url: /fr/net/aspose.cells/namecollection/remove/
---
## Remove(string[]) {#remove_1}

Supprimer un tableau de noms

```csharp
public void Remove(string[] names)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| noms | String[] | Le texte des noms. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodRemoveWithStringArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenez le NameCollection du classeur
            NameCollection names = workbook.Worksheets.Names;
            
            // Ajouter quelques plages nommées pour démontrer la suppression
            names.Add("TestRange1");
            names.Add("TestRange2");
            names.Add("TestRange3");
            
            // Préparer le tableau de noms à supprimer
            string[] namesToRemove = new string[] { "TestRange1", "TestRange3" };

            try
            {
                // Appeler la méthode Remove avec le paramètre String[]
                names.Remove(namesToRemove);
                
                Console.WriteLine("Names removed successfully:");
                foreach (string name in namesToRemove)
                {
                    Console.WriteLine(name);
                }
                
                // Afficher les noms restants
                Console.WriteLine("\nRemaining names in the collection:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("NameCollectionRemoveDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove}

Supprimer le nom.

```csharp
public void Remove(string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | Le texte du nom. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter une plage nommée
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");
            range.Name = "TestRange";
            
            // Afficher le nombre avant la suppression
            Console.WriteLine("Named ranges count before removal: " + workbook.Worksheets.Names.Count);
            
            // Supprimer la plage nommée
            workbook.Worksheets.Names.Remove("TestRange");
            
            // Afficher le nombre après la suppression
            Console.WriteLine("Named ranges count after removal: " + workbook.Worksheets.Names.Count);
        }
    }
}
```

### Voir aussi

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


