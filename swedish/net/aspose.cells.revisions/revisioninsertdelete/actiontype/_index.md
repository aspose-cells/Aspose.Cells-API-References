---
title: "RevisionInsertDelete.ActionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionInsertDelete-egenskapen. Hämtar åtgärdstypen för denna revision"
type: docs
url: /sv/net/aspose.cells.revisions/revisioninsertdelete/actiontype/
---
## RevisionInsertDelete.ActionType property

Hämtar åtgärdstypen för denna revision.

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

    public class RevisionInsertDeletePropertyActionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och aktivera revisionsspårning
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Utför operationer för att generera infognings-/borttagningsrevisioner
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteColumn(0);

            try
            {
                // Hämta revisionsloggarna
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Iterera genom alla revisionsloggar för att hitta infognings-/borttagningsrevisioner
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionInsertDelete)
                        {
                            RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                            // Visa ActionType‑egenskapens värde
                            Console.WriteLine("ActionType: " + revisionInsertDelete.ActionType);

                            // Demonstrera olika åtgärdstyper
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

                            // Visa relaterad information
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Revision type: " + revisionInsertDelete.Type);
                        }
                    }
                }

                // Spara arbetsboken med revisioner
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

### Se även

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


