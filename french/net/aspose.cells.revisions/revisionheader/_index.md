---
title: "Classe RevisionHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "La classe Aspose.Cells.Revisions.RevisionHeader représente une liste de modifications spécifiques qui ont eu lieu pour ce classeur"
type: docs
url: /fr/net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

Représente une liste de modifications spécifiques qui ont eu lieu pour ce classeur.

```csharp
public class RevisionHeader
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RevisionHeader](revisionheader/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | Obtient et définit la date et l'heure auxquelles cet ensemble de révisions a été enregistré. |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | Obtient et définit le nom de l'utilisateur effectuant la révision. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionHeaderDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créez une instance de la classe RevisionHeader
                RevisionHeader revisionHeader = new RevisionHeader();

                // Définissez les propriétés essentielles
                revisionHeader.SavedTime = DateTime.Now;
                revisionHeader.UserName = "TestUser";

                // Démontrez la fonctionnalité de base
                Console.WriteLine($"Revision saved by: {revisionHeader.UserName}");
                Console.WriteLine($"Revision saved at: {revisionHeader.SavedTime}");

                // Enregistrez le classeur
                workbook.Save("RevisionHeaderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with revision header information.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionHeader: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


