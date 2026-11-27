---
title: "Klass RevisionCellChange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionCellChange klass. Representerar revisionen som ändrar celler"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellchange/
---
## RevisionCellChange class

Representerar revisionen som ändrar celler.

```csharp
public class RevisionCellChange : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CellName](../../aspose.cells.revisions/revisioncellchange/cellname/) { get; } | Hämtar cellens namn. |
| [Column](../../aspose.cells.revisions/revisioncellchange/column/) { get; } | Hämtar kolumnindex för cellen. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| [IsNewFormatted](../../aspose.cells.revisions/revisioncellchange/isnewformatted/) { get; } | Indikerar om denna cell är nyformaterad. |
| [IsOldFormatted](../../aspose.cells.revisions/revisioncellchange/isoldformatted/) { get; } | Indikerar om denna cell är gammalformaterad. |
| [NewFormula](../../aspose.cells.revisions/revisioncellchange/newformula/) { get; } | Hämtar den gamla formeln. |
| [NewStyle](../../aspose.cells.revisions/revisioncellchange/newstyle/) { get; } | Hämtar den nya stilen för cellen. |
| [NewValue](../../aspose.cells.revisions/revisioncellchange/newvalue/) { get; } | Hämtar det nya värdet för cellen. |
| [OldFormula](../../aspose.cells.revisions/revisioncellchange/oldformula/) { get; } | Hämtar den gamla formeln. |
| [OldStyle](../../aspose.cells.revisions/revisioncellchange/oldstyle/) { get; } | Hämtar den gamla stilen för cellen. |
| [OldValue](../../aspose.cells.revisions/revisioncellchange/oldvalue/) { get; } | Hämtar det gamla värdet för cellen. |
| [Row](../../aspose.cells.revisions/revisioncellchange/row/) { get; } | Hämtar radindex för cellen. |
| override [Type](../../aspose.cells.revisions/revisioncellchange/type/) { get; } | Representerar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionsClassRevisionCellChangeDemo
    {
        public static void Run()
        {
            // Skapa utdatamapp om den inte finns
            string outputDir = "output/";
            System.IO.Directory.CreateDirectory(outputDir);
            
            string filePath = outputDir + "RevisionsClassRevisionCellChangeDemo_out.xlsx";

            // Skapa initial arbetsbok och aktivera delning
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Save(filePath, SaveFormat.Xlsx);

            // Öppna arbetsboken igen för att göra spårade ändringar
            Workbook workbook2 = new Workbook(filePath);
            Worksheet sheet = workbook2.Worksheets[0];
            
            // Första revisionen: Ställ in initiala värden
            sheet.Cells["A1"].PutValue("Initial Value");
            sheet.Cells["B2"].PutValue(100);
            workbook2.Save(filePath, SaveFormat.Xlsx);
            
            // Andra revisionen: Ändra värden
            sheet.Cells["A1"].PutValue("Updated Value");
            sheet.Cells["B2"].PutValue(200);
            workbook2.Save(filePath, SaveFormat.Xlsx);

            // Läs in arbetsboken för att komma åt revisionsloggar
            Workbook workbook3 = new Workbook(filePath);
            
            // Bearbeta alla revisionsloggar
            foreach (RevisionLog log in workbook3.Worksheets.RevisionLogs)
            {
                foreach (Revision rev in log.Revisions)
                {
                    if (rev.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange rcc = (RevisionCellChange)rev;
                        Console.WriteLine($"Revision Type: {rev.Type}");
                        Console.WriteLine($"Cell: {rcc.CellName} (Row: {rcc.Row}, Column: {rcc.Column})");
                        Console.WriteLine($"Old Value: {rcc.OldValue ?? "null"}");
                        Console.WriteLine($"New Value: {rcc.NewValue ?? "null"}");
                        Console.WriteLine("------------------------------------");
                    }
                }
            }
        }
    }
}
```

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


