---
title: "Enum PivotRefreshState"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Pivot.PivotRefreshState enum. Lo stato per l'aggiornamento delle tabelle pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotrefreshstate/
---
## PivotRefreshState enumeration

Lo stato per l'aggiornamento delle PivotTable.

```csharp
public enum PivotRefreshState
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Success | `0` | Aggiornamento riuscito |
| UnsupportedExternalDataSource | `1` | Aggiornamento fallito perché la fonte dati è esterna. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotRefreshStateDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con una tabella pivot di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Dimostra PivotRefreshState
            PivotRefreshState refreshState = pivotTable.RefreshData();
            if (refreshState == PivotRefreshState.Success)
            {
                Console.WriteLine("Pivot table refreshed successfully");
            }
            else if (refreshState == PivotRefreshState.UnsupportedExternalDataSource)
            {
                Console.WriteLine("External data source not supported - calculating data instead");
                pivotTable.CalculateData();
            }

            // Salva la cartella di lavoro
            workbook.Save("PivotRefreshStateDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


