---
title: "RevisionCustomView.ActionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCustomView-egenskap. Hämtar åtgärdstypen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncustomview/actiontype/
---
## RevisionCustomView.ActionType property

Hämtar åtgärdstypen.

```csharp
public RevisionActionType ActionType { get; }
```

### Exempel

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
                // Läs in en befintlig arbetsbok som kan innehålla anpassade vyrevisioner
                Workbook workbook = new Workbook("SampleWithRevisions.xlsx");

                // Iterera genom alla revisionsloggar i arbetsboken
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    // Kontrollera varje revision i loggen
                    foreach (Revision revision in log.Revisions)
                    {
                        // Kontrollera om detta är en anpassad vyrevision
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Visa ActionType‑egenskapens värde
                            Console.WriteLine($"Custom View Revision Action Type: {customViewRevision.ActionType}");

                            // Visa hur man använder ActionType-egenskapen
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

                            // Visa ytterligare egenskaper för kontext
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

### Se även

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


