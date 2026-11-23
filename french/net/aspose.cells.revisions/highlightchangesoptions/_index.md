---
title: "Classe HighlightChangesOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Revisions.HighlightChangesOptions class. Représente les options de mise en évidence des révisions ou des modifications des fichiers Excel partagés"
type: docs
url: /fr/net/aspose.cells.revisions/highlightchangesoptions/
---
## HighlightChangesOptions class

Représente les options de mise en évidence des révisions ou des modifications des fichiers Excel partagés.

```csharp
public class HighlightChangesOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [HighlightChangesOptions](highlightchangesoptions/)(bool, bool) | Représente les options de mise en évidence des révisions ou des modifications des fichiers Excel partagés. |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsDemo
    {
        public static void HighlightChangesExample()
        {
            // Instanciez un objet Workbook
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Obtenir les journaux de révisions
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Définir le nombre de jours pour conserver l'historique
            revisionLogs.DaysPreservingHistory = 30;

            // Créer HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // Mettre en évidence les modifications
            revisionLogs.HighlightChanges(options);

            // Enregistrez le classeur avec les modifications mises en évidence
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


