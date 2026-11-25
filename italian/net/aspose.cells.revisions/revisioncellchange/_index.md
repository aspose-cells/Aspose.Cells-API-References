---
title: "Classe RevisionCellChange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Revisions.RevisionCellChange class. Rappresenta la revisione che modifica le celle"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellchange/
---
## RevisionCellChange class

Rappresenta la revisione che modifica le celle.

```csharp
public class RevisionCellChange : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CellName](../../aspose.cells.revisions/revisioncellchange/cellname/) { get; } | Ottiene il nome della cella. |
| [Column](../../aspose.cells.revisions/revisioncellchange/column/) { get; } | Restituisce l'indice della colonna della cella. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| [IsNewFormatted](../../aspose.cells.revisions/revisioncellchange/isnewformatted/) { get; } | Indica se questa cella è formattata come nuova. |
| [IsOldFormatted](../../aspose.cells.revisions/revisioncellchange/isoldformatted/) { get; } | Indica se questa cella è formattata come vecchia. |
| [NewFormula](../../aspose.cells.revisions/revisioncellchange/newformula/) { get; } | Ottiene la formula precedente. |
| [NewStyle](../../aspose.cells.revisions/revisioncellchange/newstyle/) { get; } | Ottiene lo stile nuovo della cella. |
| [NewValue](../../aspose.cells.revisions/revisioncellchange/newvalue/) { get; } | Ottiene il nuovo valore della cella. |
| [OldFormula](../../aspose.cells.revisions/revisioncellchange/oldformula/) { get; } | Ottiene la formula precedente. |
| [OldStyle](../../aspose.cells.revisions/revisioncellchange/oldstyle/) { get; } | Ottiene lo stile vecchio della cella. |
| [OldValue](../../aspose.cells.revisions/revisioncellchange/oldvalue/) { get; } | Ottiene il valore vecchio della cella. |
| [Row](../../aspose.cells.revisions/revisioncellchange/row/) { get; } | Restituisce l'indice della riga della cella. |
| override [Type](../../aspose.cells.revisions/revisioncellchange/type/) { get; } | Rappresenta il tipo di revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

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
            // Crea la directory di output se non esiste
            string outputDir = "output/";
            System.IO.Directory.CreateDirectory(outputDir);
            
            string filePath = outputDir + "RevisionsClassRevisionCellChangeDemo_out.xlsx";

            // Crea la cartella di lavoro iniziale e abilita la condivisione
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Save(filePath, SaveFormat.Xlsx);

            // Riapri la cartella di lavoro per apportare modifiche tracciate
            Workbook workbook2 = new Workbook(filePath);
            Worksheet sheet = workbook2.Worksheets[0];
            
            // Prima revisione: Imposta i valori iniziali
            sheet.Cells["A1"].PutValue("Initial Value");
            sheet.Cells["B2"].PutValue(100);
            workbook2.Save(filePath, SaveFormat.Xlsx);
            
            // Seconda revisione: Modifica i valori
            sheet.Cells["A1"].PutValue("Updated Value");
            sheet.Cells["B2"].PutValue(200);
            workbook2.Save(filePath, SaveFormat.Xlsx);

            // Carica la cartella di lavoro per accedere ai registri delle revisioni
            Workbook workbook3 = new Workbook(filePath);
            
            // Elabora tutti i registri delle revisioni
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

### Vedi anche

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


