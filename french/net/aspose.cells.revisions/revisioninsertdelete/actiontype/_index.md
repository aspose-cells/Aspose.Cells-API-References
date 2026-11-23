---
title: "RevisionInsertDelete.ActionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionInsertDelete. Obtient le type d’action de cette révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisioninsertdelete/actiontype/
---
## RevisionInsertDelete.ActionType property

Obtient le type d'action de cette révision.

```csharp
public RevisionActionType ActionType { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyActionTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et activez le suivi des révisions
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Effectuez des opérations pour générer des révisions d’insertion/suppression
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteColumn(0);

            try
            {
                // Obtenir les journaux de révisions
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Itérez à travers tous les journaux de révisions pour trouver les révisions d’insertion/suppression
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionInsertDelete)
                        {
                            RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                            // Affichez la valeur de la propriété ActionType
                            Console.WriteLine("ActionType: " + revisionInsertDelete.ActionType);

                            // Démontrer différents types d'actions
                            switch (revisionInsertDelete.ActionType)
                            {
                                case RevisionActionType.InsertRow:
                                    Console.WriteLine("This was a row insertion operation");
                                    break;
                                case RevisionActionType.DeleteColumn:
                                    Console.WriteLine("This was a column deletion operation");
                                    break;
                                case RevisionActionType.Add:
                                    Console.WriteLine("This was an add operation");
                                    break;
                                default:
                                    Console.WriteLine("This was another type of insert/delete operation");
                                    break;
                            }

                            // Afficher les informations liées
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Revision type: " + revisionInsertDelete.Type);
                        }
                    }
                }

                // Enregistrer le classeur avec les révisions
                workbook.Save("ActionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved with revision history.");
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

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


