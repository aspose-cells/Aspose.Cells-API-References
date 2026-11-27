---
title: "Klass RevisionCustomView"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionCustomView-klass. Representerar en revisionspost för att lägga till eller ta bort en anpassad vy i arbetsboken"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncustomview/
---
## RevisionCustomView class

Representerar en revisionspost för att lägga till eller ta bort en anpassad vy i arbetsboken.

```csharp
public class RevisionCustomView : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncustomview/actiontype/) { get; } | Hämtar åtgärdstypen. |
| [Guid](../../aspose.cells.revisions/revisioncustomview/guid/) { get; } | Hämtar den globalt unika identifieraren för den anpassade vyn. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisioncustomview/type/) { get; } | Hämtar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till en anpassad vy för att eventuellt generera en revision
                // Obs: Använder CustomDocumentProperties som en lösning eftersom CustomViews inte är tillgängligt
                workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");

                // Kom åt revisionsloggarna (förutsatt att de finns)
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Visa skrivskyddade egenskaper
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Action Type: {customViewRevision.ActionType}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");

                            // Demonstrera grundläggande användning av egenskaperna
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

                // Spara arbetsboken
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

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


