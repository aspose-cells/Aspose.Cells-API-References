---
title: "Enum TotalsCalculation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Tables.TotalsCalculation. Determina il tipo di calcolo nella riga Totali della colonna dell'elenco"
type: docs
url: /it/net/aspose.cells.tables/totalscalculation/
---
## TotalsCalculation enumeration

Determina il tipo di calcolo nella riga Totali della colonna dell'elenco.

```csharp
public enum TotalsCalculation
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Sum | `6` | Rappresenta il calcolo dei totali di somma. |
| Count | `2` | Rappresenta il calcolo dei totali di conteggio. |
| Average | `1` | Rappresenta il calcolo dei totali di media. |
| Max | `4` | Rappresenta il calcolo dei totali di massimo. |
| Min | `5` | Rappresenta il calcolo dei totali Min. |
| Var | `8` | Rappresenta il calcolo dei totali Var. |
| CountNums | `3` | Rappresenta il calcolo dei totali Count Nums. |
| StdDev | `7` | Rappresenta il calcolo dei totali StdDev. |
| None | `0` | Rappresenta il calcolo dei totali No. |
| Custom | `9` | Rappresenta un calcolo personalizzato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TotalsCalculationDemo
    {
        public static void TotalsCalculationExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Popola il foglio di lavoro con alcuni dati
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Aggiungi una tabella al foglio di lavoro
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Mostra la riga dei totali
            table.ShowTotals = true;

            // Accedi alla quinta colonna nella tabella
            ListColumn listColumn = table.ListColumns[4];

            // Imposta la proprietà TotalsCalculation su Sum
            listColumn.TotalsCalculation = TotalsCalculation.Sum;

            // Facoltativamente, imposta una formula per la colonna
            listColumn.Formula = "=[A]";

            // Salva la cartella di lavoro
            workbook.Save("TotalsCalculationExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


