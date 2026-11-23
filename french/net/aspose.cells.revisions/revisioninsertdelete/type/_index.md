---
title: "RevisionInsertDelete.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionInsertDelete. Représente le type de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisioninsertdelete/type/
---
## RevisionInsertDelete.Type property

Représente le type de révision.

```csharp
public override RevisionType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et activez le suivi des révisions
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30; // Enable revision tracking by setting days

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Insérez une ligne pour générer un enregistrement de révision
            worksheet.Cells.InsertRows(0, 1);

            // Obtenez la collection de révisions (RevisionLogCollection elle-même est la collection)
            RevisionLogCollection revisions = workbook.Worksheets.RevisionLogs;

            // Trouvez le RevisionInsertDelete dans les révisions
            foreach (RevisionLog revisionLog in revisions)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Afficher la valeur de la propriété Type
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);

                        // Démontrer l’utilisation de la propriété Type
                        if (revisionInsertDelete.Type == RevisionType.InsertDelete)
                        {
                            Console.WriteLine("This revision represents an insert/delete operation");
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Action type: " + revisionInsertDelete.ActionType);
                        }

                        break;
                    }
                }
            }

            // Enregistrer le classeur avec les révisions
            workbook.Save("RevisionInsertDeletePropertyTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


