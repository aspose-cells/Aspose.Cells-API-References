---
title: "Enum PivotItemPositionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Pivot.PivotItemPositionType enum. Rappresenta il tipo di posizione dell'elemento base del pivot nel campo base quando è in uso il calcolo ShowDataAs"
type: docs
url: /it/net/aspose.cells.pivot/pivotitempositiontype/
---
## PivotItemPositionType enumeration

Rappresenta il tipo di posizione dell'elemento base pivot nel campo base quando è in uso il calcolo ShowDataAs.

```csharp
public enum PivotItemPositionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Previous | `0` | Rappresenta l'elemento pivot precedente nel PivotField. |
| Next | `1` | Rappresenta l'elemento pivot successivo nel PivotField. |
| Custom | `2` | Mostra i valori in un formato diverso basato sull'indice dell'elemento pivot nel PivotField. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotItemPositionTypeDemo
    {
        public static void PivotItemPositionTypeExample()
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

            // Aggiungi una tabella pivot al foglio di lavoro
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value

            // Imposta il formato di visualizzazione dei dati per mostrare i valori come differenza rispetto all'elemento precedente
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Previous, 0);

            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Salva la cartella di lavoro
            workbook.Save("PivotItemPositionTypeExample.xlsx");

            Console.WriteLine("Pivot table created and saved successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


