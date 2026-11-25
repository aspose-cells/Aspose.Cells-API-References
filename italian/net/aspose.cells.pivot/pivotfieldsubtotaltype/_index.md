---
title: "Enum PivotFieldSubtotalType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Pivot.PivotFieldSubtotalType enum. Descrizione riepilogativa per PivotFieldSubtotalType"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldsubtotaltype/
---
## PivotFieldSubtotalType enumeration

Descrizione riepilogativa per PivotFieldSubtotalType.

```csharp
[Flags]
public enum PivotFieldSubtotalType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Rappresenta il tipo di subtotale Nessuno. |
| Automatic | `1` | Rappresenta il tipo di subtotale Automatico. |
| Sum | `2` | Rappresenta il tipo di subtotale Somma. |
| Count | `4` | Rappresenta il tipo di subtotale Conteggio. |
| Average | `8` | Rappresenta il tipo di subtotale Media. |
| Max | `10` | Rappresenta il tipo di subtotale Massimo. |
| Min | `20` | Rappresenta il tipo di subtotale Minimo. |
| Product | `40` | Rappresenta il tipo di subtotale Prodotto. |
| CountNums | `80` | Rappresenta il tipo di subtotale Count Nums. |
| Stdev | `100` | Rappresenta il tipo di subtotale Deviazione standard. |
| Stdevp | `200` | Rappresenta il tipo di subtotale Deviazione standard di una popolazione. |
| Var | `400` | Rappresenta il tipo di subtotale Varianza. |
| Varp | `800` | Rappresenta il tipo di subtotale Varianza di una popolazione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSubtotalTypeDemo
    {
        public static void PivotFieldSubtotalTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Aggiungi una tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Imposta il tipo di subtotale per il campo di riga
            PivotField rowField = pivotTable.RowFields[0];
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            rowField.SetSubtotals(PivotFieldSubtotalType.Count, true);

            // Aggiorna e calcola i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldSubtotalTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


