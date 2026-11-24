---
title: "RevisionCustomView.ActionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCustomView-Eigenschaft. Gibt den Typ der Aktion zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncustomview/actiontype/
---
## RevisionCustomView.ActionType property

Ruft den Aktionstyp ab.

```csharp
public RevisionActionType ActionType { get; }
```

### Beispiele

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
                // Laden Sie eine vorhandene Arbeitsmappe, die benutzerdefinierte Ansichtrevisionen enthalten könnte
                Workbook workbook = new Workbook("SampleWithRevisions.xlsx");

                // Durchlaufen Sie alle Revisionsprotokolle in der Arbeitsmappe
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    // Überprüfen Sie jede Revision im Protokoll
                    foreach (Revision revision in log.Revisions)
                    {
                        // Prüfen Sie, ob dies eine benutzerdefinierte Ansichtrevision ist
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Zeigen Sie den Wert der ActionType-Eigenschaft an
                            Console.WriteLine($"Custom View Revision Action Type: {customViewRevision.ActionType}");

                            // Demonstrieren Sie, wie die ActionType-Eigenschaft verwendet wird
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

                            // Zusätzliche Eigenschaften für den Kontext anzeigen
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

### Siehe auch

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


