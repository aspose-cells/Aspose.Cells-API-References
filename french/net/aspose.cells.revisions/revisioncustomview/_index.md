---
title: "Classe RevisionCustomView"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Revisions.RevisionCustomView. Représente un enregistrement de révision d'ajout ou de suppression d'une vue personnalisée au classeur"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncustomview/
---
## RevisionCustomView class

Représente un enregistrement de révision d'ajout ou de suppression d'une vue personnalisée au classeur.

```csharp
public class RevisionCustomView : Revision
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncustomview/actiontype/) { get; } | Obtient le type d'action. |
| [Guid](../../aspose.cells.revisions/revisioncustomview/guid/) { get; } | Obtient l'identifiant unique global de la vue personnalisée. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtient le numéro de cette révision.(Hérité de [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisioncustomview/type/) { get; } | Obtient le type de révision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtient la feuille de calcul. (Hérité de [`Revision`](../revision/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCustomViewDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajoutez une vue personnalisée pour potentiellement générer une révision
                // Remarque : utilisation de CustomDocumentProperties comme solution de contournement puisque CustomViews n'est pas disponible
                workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");

                // Accédez aux journaux de révision (en supposant qu'ils existent)
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Affichez les propriétés en lecture seule
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Action Type: {customViewRevision.ActionType}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");

                            // Démontrez l'utilisation de base des propriétés
                            if (customViewRevision.Type == RevisionType.CustomView)
                            {
                                Console.WriteLine("This is a custom view revision.");
                            }

                            if (customViewRevision.ActionType == RevisionActionType.Add)
                            {
                                Console.WriteLine("The custom view was added.");
                            }
                            else if (customViewRevision.ActionType == RevisionActionType.Delete)
                            {
                                Console.WriteLine("The custom view was deleted.");
                            }
                        }
                    }
                }

                // Enregistrez le classeur
                workbook.Save("RevisionCustomViewDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


