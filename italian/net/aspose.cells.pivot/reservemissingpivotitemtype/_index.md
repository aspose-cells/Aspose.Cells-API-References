---
title: "Enum ReserveMissingPivotItemType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Pivot.ReserveMissingPivotItemType enum. Rappresenta come mantenere gli elementi pivot mancanti"
type: docs
url: /it/net/aspose.cells.pivot/reservemissingpivotitemtype/
---
## ReserveMissingPivotItemType enumeration

Rappresenta come mantenere gli elementi pivot mancanti.

```csharp
public enum ReserveMissingPivotItemType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Rimuove i vecchi elementi pivot mancanti e riserva gli elementi eliminati della nuova origine dati come elementi mancanti. |
| All | `1` | Riserva tutti gli elementi mancanti. |
| None | `2` | Rimuove tutti gli elementi pivot mancanti. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class ReserveMissingPivotItemTypeDemo
    {
        public static void ReserveMissingPivotItemTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi una PivotTable al foglio di lavoro
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Aggiungi campi alla PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Imposta l'opzione ReserveMissingPivotItemType
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calcola la PivotTable con le opzioni specificate
            pivotTable.CalculateData(calculateOption);

            // Aggiorna la PivotTable
            pivotTable.RefreshData();

            // Salva la cartella di lavoro
            workbook.Save("ReserveMissingPivotItemTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


