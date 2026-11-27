---
title: "RevisionCellChange.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellChange-egenskap. Representerar revisionstypen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellchange/type/
---
## RevisionCellChange.Type property

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

    public class RevisionCellChangePropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aktivera spårning av ändringar genom att modifiera en cell – revisioner spåras automatiskt
            // när ändringar görs efter att arbetsboken skapats
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Initial Value");

            // Ändra cellen för att skapa en revision
            cell.PutValue("Modified Value");

            // Åtkomst till revisionsloggarna
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Visa typinformation från revisionen
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Revision Type: " + cellChange.Type);

                        // Demonstrera användning av Type‑egenskapen
                        if (cellChange.Type == RevisionType.ChangeCells)
                        {
                            Console.WriteLine("\nThis is a cell change revision");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }

                        // Kontrollera andra möjliga revisionstyper
                        switch (cellChange.Type)
                        {
                            case RevisionType.ChangeCells:
                                Console.WriteLine("Handling cell value change revision");
                                break;
                            case RevisionType.Format:
                                Console.WriteLine("Handling format change revision");
                                break;
                            default:
                                Console.WriteLine("Handling other type of revision");
                                break;
                        }
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellChangePropertyTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


