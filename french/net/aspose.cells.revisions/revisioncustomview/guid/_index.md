---
title: "RevisionCustomView.Guid"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCustomView. Obtient l'identifiant unique global de la vue personnalisée"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncustomview/guid/
---
## RevisionCustomView.Guid property

Obtient l'identifiant unique global de la vue personnalisée.

```csharp
public Guid Guid { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCustomViewPropertyGuidDemo
    {
        public static void Run()
        {
            // Ouvrir un classeur existant qui contient des révisions de vue personnalisée
            Workbook workbook = new Workbook("example.xlsx");
            
            // Traiter les journaux de révision
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.CustomView)
                    {
                        RevisionCustomView rcv = (RevisionCustomView)revision;
                        Console.WriteLine($"ActionType: {rcv.ActionType}, Guid: {rcv.Guid}");
                    }
                }
            }
        }
    }
}
```

### Voir aussi

* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


