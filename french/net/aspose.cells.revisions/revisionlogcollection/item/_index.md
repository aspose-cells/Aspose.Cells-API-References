---
title: "RevisionLogCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionLogCollection. Obtient RevisionLog par indice"
type: docs
url: /fr/net/aspose.cells.revisions/revisionlogcollection/item/
---
## RevisionLogCollection indexer

Obtient [`RevisionLog`](../../revisionlog/) par indice.

```csharp
public RevisionLog this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

Renvoie l'objet [`RevisionLog`](../../revisionlog/).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Activer le classeur partagé pour prendre en charge les révisions
            workbook.Settings.Shared = true;

            // Accédez à la collection des journaux de révision
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            try
            {
                // Vérifier s'il existe des journaux de révision
                if (revisionLogs.Count > 0)
                {
                    // Accéder au premier journal de révision en utilisant la propriété Item
                    RevisionLog firstLog = revisionLogs[0];

                    // Afficher les informations de base sur le journal de révision
                    Console.WriteLine("First revision log accessed via Item property:");
                    Console.WriteLine($"Revision count: {firstLog.Revisions.Count}");
                }
                else
                {
                    Console.WriteLine("No revision logs available in the workbook.");
                }

                // Enregistrez le classeur
                workbook.Save("RevisionLogItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [RevisionLog](../../revisionlog/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


