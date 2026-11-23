---
title: "RevisionCellChange.NewValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCellChange. Obtient la nouvelle valeur de la cellule"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncellchange/newvalue/
---
## RevisionCellChange.NewValue property

Obtient la nouvelle valeur de la cellule.

```csharp
public object NewValue { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données initiales à la cellule A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");

            // Modifiez la cellule pour créer une révision
            cell.PutValue("Modified Value");

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
                            // Affichez la propriété NewValue
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Démontrez l'utilisation de la propriété NewValue
                            if (cellChange.NewValue != null)
                            {
                                Console.WriteLine("\nThe new value is: " + cellChange.NewValue.ToString());
                            }
                        }
                    }
                }

                // Enregistrer le classeur avec les révisions
                workbook.Save("RevisionCellChangePropertyNewValueDemo.xlsx");
                Console.WriteLine("\nWorkbook saved with revisions.");
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


