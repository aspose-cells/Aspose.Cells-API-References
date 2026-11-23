---
title: "RevisionHeader.UserName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionHeader. Obtient et définit le nom de l'utilisateur effectuant la révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

Obtient et définit le nom de l'utilisateur effectuant la révision.

```csharp
public string UserName { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertyUserNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Créer une instance de RevisionHeader
                RevisionHeader revisionHeader = new RevisionHeader();

                // Définir la propriété UserName
                revisionHeader.UserName = "JohnDoe";

                // Afficher la valeur actuelle de la propriété UserName
                Console.WriteLine("UserName value: " + revisionHeader.UserName);

                // Modifier la propriété UserName
                revisionHeader.UserName = "JaneSmith";
                Console.WriteLine("Modified UserName value: " + revisionHeader.UserName);

                // Enregistrer le classeur pour démontrer que la propriété est utilisée
                workbook.Save("UserNameDemo.xlsx");
                Console.WriteLine("UserName property has been demonstrated and workbook saved.");
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


