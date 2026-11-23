---
title: "RevisionCellChange.Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellChange. Obtient l'index de colonne de la cellule"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellchange/column/
---
## RevisionCellChange.Column property

Obtient l'index de colonne de la cellule.

```csharp
public int Column { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec suivi des révisions
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Modifier la cellule B2 pour générer une révision
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Initial Value");

            // Changez la cellule pour créer une révision
            cell.PutValue("Modified Value");

            // Accédez aux journaux de révision
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Afficher les informations de colonne de la révision
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Column Index: " + cellChange.Column);
                        Console.WriteLine("Row Index: " + cellChange.Row);

                        // Démontrer l'utilisation de la propriété Column
                        if (cellChange.Column == 1) // Column B is index 1
                        {
                            Console.WriteLine("\nThis revision affects column B");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionCellChangePropertyColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


