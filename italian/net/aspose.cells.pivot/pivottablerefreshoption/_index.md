---
title: "Classe PivotTableRefreshOption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotTableRefreshOption. Rappresenta le opzioni di aggiornamento della fonte dati della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottablerefreshoption/
---
## PivotTableRefreshOption class

Rappresenta le opzioni di aggiornamento dell'origine dati della tabella pivot.

```csharp
public class PivotTableRefreshOption
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PivotTableRefreshOption](pivottablerefreshoption/)() | Rappresenta le opzioni di aggiornamento dell'origine dati della tabella pivot. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsKeepOriginalOrder](../../aspose.cells.pivot/pivottablerefreshoption/iskeeporiginalorder/) { get; set; } | Indica se mantenere l'ordine originale degli elementi pivot come nella vecchia fonte dati. |
| [KeepCachedLocalGroupData](../../aspose.cells.pivot/pivottablerefreshoption/keepcachedlocalgroupdata/) { get; set; } | Indica se mantenere i dati di gruppo locali nella cache se i valori massimo e minimo rimangono invariati. Il valore predefinito è false, il che significa aggiornare il gruppo con impostazioni locali. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablerefreshoption/reservemissingpivotitemtype/) { get; set; } | Rappresenta come riservare gli elementi pivot mancanti. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableRefreshOptionDemo
    {
        public static void PivotTableRefreshOptionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Aggiungi una tabella pivot al foglio di lavoro
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Crea un'istanza di PivotTableRefreshOption
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Aggiorna la tabella pivot con le opzioni specificate
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTableRefreshOptionExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


