---
title: "Classe PivotTableCalculateOption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotTableCalculateOption. Rappresenta le opzioni di calcolo dei dati della tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottablecalculateoption/
---
## PivotTableCalculateOption class

Rappresenta le opzioni di calcolo dei dati della tabella pivot.

```csharp
public class PivotTableCalculateOption
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PivotTableCalculateOption](pivottablecalculateoption/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [RefreshCharts](../../aspose.cells.pivot/pivottablecalculateoption/refreshcharts/) { get; set; } | Indica se i grafici di aggiornamento si basano su questa tabella pivot. |
| [RefreshData](../../aspose.cells.pivot/pivottablecalculateoption/refreshdata/) { get; set; } | Indica se la fonte dati della tabella pivot viene aggiornata. |
| [RefreshOption](../../aspose.cells.pivot/pivottablecalculateoption/refreshoption/) { get; set; } | Ottiene e imposta le opzioni per l'aggiornamento della fonte dati nella cache della tabella pivot. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/) { get; set; } | Rappresenta come riservare gli elementi pivot mancanti. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionDemo
    {
        public static void PivotTableCalculateOptionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per la tabella pivot
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // Aggiungi una tabella pivot al foglio di lavoro
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Crea un oggetto PivotTableCalculateOption
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calcola i dati della tabella pivot con le opzioni specificate
            pivotTable.CalculateData(calculateOption);

            // Salva la cartella di lavoro
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


