---
title: "Class RevisionAutoFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "La classe Aspose.Cells.Revisions.RevisionAutoFormat représente un enregistrement de révision d'informations sur une modification de formatage."
type: docs
url: /fr/net/aspose.cells.revisions/revisionautoformat/
---
## RevisionAutoFormat class

représente un enregistrement de révision d'informations sur une modification de formatage.

```csharp
public class RevisionAutoFormat : Revision
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionautoformat/cellarea/) { get; } | Obtient l'emplacement où le formatage a été appliqué. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtient le numéro de cette révision.(Hérité de [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionautoformat/type/) { get; } | Obtient le type de la révision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtient la feuille de calcul. (Hérité de [`Revision`](../revision/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionAutoFormatDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();

            try
            {
                // Accédez à la collection des journaux de révision
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Trouvez la première instance de RevisionAutoFormat
                RevisionAutoFormat revisionFormat = null;
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionAutoFormat)
                        {
                            revisionFormat = (RevisionAutoFormat)revision;
                            break;
                        }
                    }
                    if (revisionFormat != null) break;
                }

                if (revisionFormat != null)
                {
                    // Démontrez la propriété Type (lecture seule)
                    RevisionType type = revisionFormat.Type;
                    Console.WriteLine($"Revision type: {type}");

                    // Démontrez la propriété CellArea (lecture seule)
                    CellArea area = revisionFormat.CellArea;
                    Console.WriteLine($"Formatting applied to area: StartRow={area.StartRow}, " +
                                      $"StartColumn={area.StartColumn}, EndRow={area.EndRow}, " +
                                      $"EndColumn={area.EndColumn}");
                }
                else
                {
                    Console.WriteLine("No auto-format revisions found in the workbook");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionAutoFormat: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


