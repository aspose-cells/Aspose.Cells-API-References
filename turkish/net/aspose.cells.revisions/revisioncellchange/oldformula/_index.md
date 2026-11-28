---
title: "RevisionCellChange.OldFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCellChange özelliği. Eski formülü alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncellchange/oldformula/
---
## RevisionCellChange.OldFormula property

Eski formülü alır.

```csharp
public string OldFormula { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCellChangePropertyOldFormulaDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook("example.xlsx");
            if (!wb.HasRevisions)
            {
                Console.WriteLine("No revisions found.");
                return;
            }

            RevisionLogCollection logs = wb.Worksheets.RevisionLogs;
            Console.WriteLine($"Found {logs.Count} revision logs");

            int formulaCount = 0;
            foreach (RevisionLog log in logs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        string formula = cellChange.OldFormula;
                        
                        if (formula != null)
                        {
                            Console.WriteLine($"Cell {cellChange.CellName} had formula: {formula}");
                            if ((cellChange.Row == 0 && formula == "Sheet2!A1") || 
                                (cellChange.Row == 1 && formula == "Sheet2!#REF!"))
                            {
                                formulaCount++;
                            }
                        }
                    }
                }
            }
            
            Console.WriteLine($"Matched {formulaCount} formula changes");
        }
    }
}
```

### Ayrıca Bakınız

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


