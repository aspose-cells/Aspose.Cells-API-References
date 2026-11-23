---
title: "RevisionInsertSheet.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionInsertSheet. Obtient le nom de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.revisions/revisioninsertsheet/name/
---
## RevisionInsertSheet.Name property

Obtient le nom de la feuille de calcul.

```csharp
public string Name { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajoutez une nouvelle feuille de calcul pour potentiellement générer un enregistrement de révision
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

            try
            {
                // Simuler l'accès à un RevisionInsertSheet depuis les révisions
                // Remarque : dans un scénario réel, cela proviendrait de workbook.Revisions
                // À des fins de démonstration, nous créerons un scénario factice
                RevisionInsertSheet insertSheetRevision = null;

                // Dans une utilisation réelle, vous obtiendriez cela à partir de la collection de révisions
                // Par exemple : insertSheetRevision = (RevisionInsertSheet)workbook.Revisions[0];

                // Comme nous ne pouvons pas créer directement un RevisionInsertSheet, nous allons le démontrer
                // ce que vous feriez si vous aviez accès à un
                if (insertSheetRevision != null)
                {
                    // Afficher la valeur de la propriété Name (lecture seule)
                    Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);

                    // Démontrer l'utilisation de la propriété Name dans une condition
                    if (!string.IsNullOrEmpty(insertSheetRevision.Name))
                    {
                        Console.WriteLine("The sheet has a valid name: " + insertSheetRevision.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No RevisionInsertSheet found in revisions");
                }

                // Enregistrez le classeur
                workbook.Save("RevisionInsertSheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


