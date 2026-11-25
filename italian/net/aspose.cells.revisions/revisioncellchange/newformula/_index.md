---
title: "RevisionCellChange.NewFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellChange. Ottiene la vecchia formula"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellchange/newformula/
---
## RevisionCellChange.NewFormula property

Ottiene la formula precedente.

```csharp
public string NewFormula { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta la formula iniziale nella cella A1
            worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Modifica la formula per creare una revisione
            worksheet.Cells["A1"].Formula = "=AVERAGE(B1:B3)";

            // Accedi ai registri delle revisioni
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
                    {
                        // Visualizza le informazioni sulla modifica della formula
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Formula: " + cellChange.OldFormula);
                        Console.WriteLine("New Formula: " + cellChange.NewFormula);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Dimostra l'uso della proprietà NewFormula
                        if (!string.IsNullOrEmpty(cellChange.NewFormula))
                        {
                            Console.WriteLine("\nThe cell's new formula calculates: " + 
                                worksheet.Cells["A1"].StringValue);
                        }
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellChangePropertyNewFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


