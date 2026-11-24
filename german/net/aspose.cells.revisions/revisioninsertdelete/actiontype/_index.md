---
title: "RevisionInsertDelete.ActionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionInsertDelete-Eigenschaft. Gibt den Aktionstyp dieser Revision zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioninsertdelete/actiontype/
---
## RevisionInsertDelete.ActionType property

Ermittelt den Aktionstyp dieser Revision.

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

    public class RevisionInsertDeletePropertyActionTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch und aktiviere die Revisionsverfolgung
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Führe Vorgänge aus, um Einfügungs-/Löschungsrevisionen zu erzeugen
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteColumn(0);

            try
            {
                // Rufe die Revisionsprotokolle ab
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Iteriere über alle Revisionsprotokolle, um Einfügungs- und Löschungsrevisionen zu finden
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionInsertDelete)
                        {
                            RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                            // Zeigen Sie den Wert der ActionType-Eigenschaft an
                            Console.WriteLine("ActionType: " + revisionInsertDelete.ActionType);

                            // Demonstriere verschiedene Aktionstypen
                            switch (revisionInsertDelete.ActionType)
                            {
                                case RevisionActionType.InsertRow:
                                    Console.WriteLine("This was a row insertion operation");
                                    break;
                                case RevisionActionType.DeleteColumn:
                                    Console.WriteLine("This was a column deletion operation");
                                    break;
                                case RevisionActionType.Add:
                                    Console.WriteLine("This was an add operation");
                                    break;
                                default:
                                    Console.WriteLine("This was another type of insert/delete operation");
                                    break;
                            }

                            // Zeige zugehörige Informationen
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Revision type: " + revisionInsertDelete.Type);
                        }
                    }
                }

                // Speichern Sie die Arbeitsmappe mit Revisionen
                workbook.Save("ActionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved with revision history.");
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
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


