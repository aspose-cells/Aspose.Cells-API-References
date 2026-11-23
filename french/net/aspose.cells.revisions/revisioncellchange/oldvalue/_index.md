---
title: "RevisionCellChange.OldValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellChange. Obtient l'ancienne valeur de la cellule"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellchange/oldvalue/
---
## RevisionCellChange.OldValue property

Obtient l'ancienne valeur de la cellule.

```csharp
public object OldValue { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyOldValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données initiales pour créer une révision
            worksheet.Cells["A1"].PutValue("Original Value");

            // Modifiez la cellule pour créer une révision
            worksheet.Cells["A1"].PutValue("Modified Value");

            try
            {
                // Accédez aux journaux de révision
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // Afficher la valeur de la propriété OldValue
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Démontrer l'utilisation de la propriété OldValue
                            if (cellChange.OldValue != null)
                            {
                                Console.WriteLine("\nThe cell was previously set to: " + cellChange.OldValue);
                            }
                        }
                    }
                }

                // Enregistrez le classeur
                workbook.Save("RevisionCellChangePropertyOldValueDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


