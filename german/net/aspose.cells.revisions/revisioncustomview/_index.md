---
title: "Klasse RevisionCustomView"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionCustomView Klasse. Stellt einen Revisionsdatensatz für das Hinzufügen oder Entfernen einer benutzerdefinierten Ansicht zur Arbeitsmappe dar"
type: docs
url: /de/net/aspose.cells.revisions/revisioncustomview/
---
## RevisionCustomView class

Stellt einen Revisionsdatensatz für das Hinzufügen oder Entfernen einer benutzerdefinierten Ansicht zum Arbeitsbuch dar.

```csharp
public class RevisionCustomView : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncustomview/actiontype/) { get; } | Ruft den Aktionstyp ab. |
| [Guid](../../aspose.cells.revisions/revisioncustomview/guid/) { get; } | Ruft die global eindeutige Kennung der benutzerdefinierten Ansicht ab. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisioncustomview/type/) { get; } | Liest den Typ der Revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

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
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Füge eine benutzerdefinierte Ansicht hinzu, um möglicherweise eine Revision zu erzeugen
                // Hinweis: Verwende CustomDocumentProperties als Umgehungslösung, da CustomViews nicht verfügbar ist
                workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");

                // Greife auf die Revisionsprotokolle zu (vorausgesetzt, sie existieren)
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Zeige die schreibgeschützten Eigenschaften an
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Action Type: {customViewRevision.ActionType}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");

                            // Demonstrieren Sie die grundlegende Verwendung der Eigenschaften
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

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


