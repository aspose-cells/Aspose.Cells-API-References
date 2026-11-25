---
title: "Enum PivotAreaType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Pivot.PivotAreaType. Indica il tipo di regola utilizzata per descrivere un'area o un aspetto della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivotareatype/
---
## PivotAreaType enumeration

Indica il tipo di regola utilizzata per descrivere un'area o un aspetto della PivotTable.

```csharp
public enum PivotAreaType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna area Pivot. |
| Normal | `1` | Rappresenta un'intestazione o un elemento. |
| Data | `2` | Rappresenta qualcosa nell'area dati. |
| All | `3` | Rappresenta l'intera PivotTable. |
| Origin | `4` | Rappresenta le celle vuote in alto a sinistra della PivotTable (in alto a destra per fogli RTL). |
| Button | `5` | Rappresenta un pulsante di campo. |
| TopRight | `6` | Rappresenta le celle vuote in alto a destra della PivotTable (in alto a sinistra per fogli RTL). |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaTypeDemo
    {
        public static void PivotAreaTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["A4"].PutValue("Bananas");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);

            // Crea una PivotTable
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Aggiungi campi alla PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Crea un PivotArea per la PivotTable
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true;
            pivotArea.IsRowGrandIncluded = true;

            // Restituisci le proprietà del PivotArea
            Console.WriteLine("Pivot Area Type: " + pivotArea.RuleType);
            Console.WriteLine("Only Data: " + pivotArea.OnlyData);
            Console.WriteLine("Is Row Grand Included: " + pivotArea.IsRowGrandIncluded);

            // Salva la cartella di lavoro
            workbook.Save("PivotAreaTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


