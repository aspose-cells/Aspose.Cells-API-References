---
title: "RevisionCustomView.ActionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RevisionCustomView. Obtient le type d'action"
type: docs
url: /fr/net/aspose.cells.revisions/revisioncustomview/actiontype/
---
## RevisionCustomView.ActionType property

Obtient le type d'action.

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

    public class RevisionCustomViewPropertyActionTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Charger un Workbook existant qui pourrait contenir des révisions de vue personnalisée
                Workbook workbook = new Workbook("SampleWithRevisions.xlsx");

                // Itérer à travers tous les journaux de révision dans le Workbook
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    // Vérifier chaque révision dans le journal
                    foreach (Revision revision in log.Revisions)
                    {
                        // Vérifier si c'est une révision de vue personnalisée
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Affichez la valeur de la propriété ActionType
                            Console.WriteLine($"Custom View Revision Action Type: {customViewRevision.ActionType}");

                            // Démontrer comment utiliser la propriété ActionType
                            switch (customViewRevision.ActionType)
                            {
                                case RevisionActionType.Add:
                                    Console.WriteLine("This revision represents adding a custom view");
                                    break;
                                case RevisionActionType.Delete:
                                    Console.WriteLine("This revision represents deleting a custom view");
                                    break;
                                default:
                                    Console.WriteLine("This revision represents another type of action");
                                    break;
                            }

                            // Afficher des propriétés supplémentaires pour le contexte
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");
                        }
                    }
                }
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
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


