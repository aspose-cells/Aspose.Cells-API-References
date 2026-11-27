---
title: "RevisionInsertDelete.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionInsertDelete-egenskapen. Representerar revisionens typ"
type: docs
url: /sv/net/aspose.cells.revisions/revisioninsertdelete/type/
---
## RevisionInsertDelete.Type property

Representerar typen av revision.

```csharp
public override RevisionType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och aktivera spårning av revisioner
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30; // Enable revision tracking by setting days

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Infoga en rad för att skapa en revisionspost
            worksheet.Cells.InsertRows(0, 1);

            // Hämta revisionssamlingen (RevisionLogCollection är själva samlingen)
            RevisionLogCollection revisions = workbook.Worksheets.RevisionLogs;

            // Hitta RevisionInsertDelete i revisionerna
            foreach (RevisionLog revisionLog in revisions)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Visa värdet för Type-egenskapen
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);

                        // Demonstrera användning av Type‑egenskapen
                        if (revisionInsertDelete.Type == RevisionType.InsertDelete)
                        {
                            Console.WriteLine("This revision represents an insert/delete operation");
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Action type: " + revisionInsertDelete.ActionType);
                        }

                        break;
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionInsertDeletePropertyTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


