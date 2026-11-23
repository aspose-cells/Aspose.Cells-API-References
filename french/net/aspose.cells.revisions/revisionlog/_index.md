---
title: "Classe RevisionLog"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Revisions.RevisionLog. Représente le journal de révision"
type: docs
url: /fr/net/aspose.cells.revisions/revisionlog/
---
## RevisionLog class

Représente le journal des révisions.

```csharp
public class RevisionLog
```

## Propriétés

| Nom | Description |
| --- | --- |
| [MetadataTable](../../aspose.cells.revisions/revisionlog/metadatatable/) { get; } | Obtient la table qui contient les métadonnées concernant une liste de modifications spécifiques survenues pour ce classeur. |
| [Revisions](../../aspose.cells.revisions/revisionlog/revisions/) { get; } | Obtient toutes les révisions de ce journal. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogDemo
    {
        public static void RevisionLogExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Accédez aux journaux de révision du classeur
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Vérifier s'il existe des journaux de révision
            if (revisionLogs.Count > 0)
            {
                // Accédez au premier journal de révision
                RevisionLog revisionLog = revisionLogs[0];

                // Accédez à la table des métadonnées du journal de révision
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // Accédez aux révisions du journal de révision
                RevisionCollection revisions = revisionLog.Revisions;

                // Affichez certaines informations sur les révisions
                Console.WriteLine("Number of revisions: " + revisions.Count);
                Console.WriteLine("Metadata Table: " + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine("No revision logs found.");
            }

            // Enregistrez le classeur
            workbook.Save("RevisionLogExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


