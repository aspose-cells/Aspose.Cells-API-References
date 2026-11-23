---
title: "RevisionHeader.SavedTime"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionHeader. Obtient et définit la date et l'heure auxquelles cet ensemble de révisions a été enregistré"
type: docs
url: /fr/net/aspose.cells.revisions/revisionheader/savedtime/
---
## RevisionHeader.SavedTime property

Obtient et définit la date et l'heure auxquelles cet ensemble de révisions a été enregistré.

```csharp
public DateTime SavedTime { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertySavedTimeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer une instance de RevisionHeader
            RevisionHeader revisionHeader = new RevisionHeader();
            
            try
            {
                // Définir la propriété SavedTime
                revisionHeader.SavedTime = DateTime.Now;
                
                // Obtenir et afficher la valeur de SavedTime
                Console.WriteLine("SavedTime value: " + revisionHeader.SavedTime);
                
                // Modifier la propriété SavedTime
                revisionHeader.SavedTime = DateTime.Now.AddHours(-1);
                Console.WriteLine("Modified SavedTime value: " + revisionHeader.SavedTime);
                
                // Enregistrer le classeur pour démontrer que la propriété est utilisée
                workbook.Save("SavedTimeDemo.xlsx");
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

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


