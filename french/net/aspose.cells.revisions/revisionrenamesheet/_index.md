---
title: "Classe RevisionRenameSheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Revisions.RevisionRenameSheet. Représente une révision du renommage de feuille"
type: docs
url: /fr/net/aspose.cells.revisions/revisionrenamesheet/
---
## RevisionRenameSheet class

Représente une révision du renommage d'une feuille.

```csharp
public class RevisionRenameSheet : Revision
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtient le numéro de cette révision.(Hérité de [`Revision`](../revision/).) |
| [NewName](../../aspose.cells.revisions/revisionrenamesheet/newname/) { get; } | Obtient le nouveau nom de la feuille de calcul. |
| [OldName](../../aspose.cells.revisions/revisionrenamesheet/oldname/) { get; } | Obtient l'ancien nom de la feuille de calcul. |
| override [Type](../../aspose.cells.revisions/revisionrenamesheet/type/) { get; } | Représente le type de la révision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtient la feuille de calcul. (Hérité de [`Revision`](../revision/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionRenameSheetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Enregistrer le nom original et renommer la feuille
                string originalName = worksheet.Name;
                worksheet.Name = "RenamedSheet";

                // Enregistrer dans un flux mémoire pour générer des révisions
                System.IO.MemoryStream ms = new System.IO.MemoryStream();
                workbook.Save(ms, SaveFormat.Xlsx);

                // Rouvrir le classeur pour accéder aux journaux de révisions
                workbook = new Workbook(ms);

                // Vérifier les journaux de révisions pour l'opération de renommage
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rv in log.Revisions)
                    {
                        if (rv.Type == RevisionType.RenameSheet)
                        {
                            RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                            Console.WriteLine("Revision Type: " + renameSheet.Type);
                            Console.WriteLine("Old Sheet Name: " + renameSheet.OldName);
                            Console.WriteLine("New Sheet Name: " + renameSheet.NewName);
                        }
                    }
                }

                // Enregistrez le classeur
                workbook.Save("RevisionRenameSheetDemo.xlsx");
                Console.WriteLine("RevisionRenameSheet demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RevisionRenameSheet demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


