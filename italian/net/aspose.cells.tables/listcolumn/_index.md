---
title: "Classe ListColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Tables.ListColumn classe. Rappresenta una colonna in una tabella"
type: docs
url: /it/net/aspose.cells.tables/listcolumn/
---
## ListColumn class

Rappresenta una colonna in una Tabella.

```csharp
public class ListColumn
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Formula](../../aspose.cells.tables/listcolumn/formula/) { get; set; } | Ottiene e imposta la formula della colonna dell'elenco. |
| [IsArrayFormula](../../aspose.cells.tables/listcolumn/isarrayformula/) { get; } | Indica se la formula è una formula di matrice. |
| [Name](../../aspose.cells.tables/listcolumn/name/) { get; set; } | Ottiene e imposta il nome della colonna. |
| [Range](../../aspose.cells.tables/listcolumn/range/) { get; } | Ottiene l'intervallo di questa colonna dell'elenco. |
| [TotalsCalculation](../../aspose.cells.tables/listcolumn/totalscalculation/) { get; set; } | Ottiene e imposta il tipo di calcolo nella riga Totali della colonna dell'elenco. |
| [TotalsRowLabel](../../aspose.cells.tables/listcolumn/totalsrowlabel/) { get; set; } | Ottiene e imposta le etichette di visualizzazione della riga totale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/getcustomcalculatedformula/)(bool, bool) | Ottiene la formula di questa colonna dell'elenco. |
| [GetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/getcustomtotalsrowformula/)(bool, bool) | Ottiene la formula della riga dei totali di questa colonna dell'elenco. |
| [GetDataStyle](../../aspose.cells.tables/listcolumn/getdatastyle/)() | Ottiene lo stile dei dati in questa colonna della tabella. |
| [SetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/setcustomcalculatedformula/)(string, bool, bool) | Imposta la formula per questa colonna dell'elenco. |
| [SetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/setcustomtotalsrowformula/)(string, bool, bool) | Ottiene la formula della riga dei totali di questa colonna dell'elenco. |
| [SetDataStyle](../../aspose.cells.tables/listcolumn/setdatastyle/)(Style) | Imposta lo stile dei dati in questa colonna della tabella. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnDemo
    {
        public static void ListColumnExample()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

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

            // Aggiungi un ListObject (tabella) al foglio di lavoro
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];
            table.ShowTotals = true;

            // Accedi al **ListColumn** e imposta le sue proprietà
            ListColumn listColumn = table.ListColumns[4];
            listColumn.TotalsCalculation = TotalsCalculation.Sum;
            listColumn.Formula = "=[A]";
            listColumn.Name = "CustomColumn";
            listColumn.TotalsRowLabel = "Total";

            // Salva la cartella di lavoro
            workbook.Save("ListColumnExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


