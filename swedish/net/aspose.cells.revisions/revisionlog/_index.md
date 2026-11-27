---
title: "Klass RevisionLog"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionLog-klass. Representerar revisionsloggen"
type: docs
url: /sv/net/aspose.cells.revisions/revisionlog/
---
## RevisionLog class

Representerar revisionsloggen.

```csharp
public class RevisionLog
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [MetadataTable](../../aspose.cells.revisions/revisionlog/metadatatable/) { get; } | Hämtar tabellen som innehåller metadata om en lista med specifika ändringar som har inträffat för den här arbetsboken. |
| [Revisions](../../aspose.cells.revisions/revisionlog/revisions/) { get; } | Hämtar alla revisioner i den här loggen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogDemo
    {
        public static void RevisionLogExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Åtkomst till revisionsloggarna för arbetsboken
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Kontrollera om det finns några revisionsloggar
            if (revisionLogs.Count > 0)
            {
                // Åtkomst till den första revisionsloggen
                RevisionLog revisionLog = revisionLogs[0];

                // Åtkomst till metadatatabellen för revisionsloggen
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // Åtkomst till revisionerna i revisionsloggen
                RevisionCollection revisions = revisionLog.Revisions;

                // Visa viss information om revisionerna
                Console.WriteLine("Number of revisions: " + revisions.Count);
                Console.WriteLine("Metadata Table: " + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine("No revision logs found.");
            }

            // Spara arbetsboken
            workbook.Save("RevisionLogExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


