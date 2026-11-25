---
title: "PivotTable.RefreshDataOnOpeningFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Indica se aggiornare i dati all'apertura del file"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/refreshdataonopeningfile/
---
## PivotTable.RefreshDataOnOpeningFile property

Indica se aggiornare i dati all'apertura del file.

```csharp
public bool RefreshDataOnOpeningFile { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshDataOnOpeningFileDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Banana";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Orange";
            cells["B4"].Value = 3000;

            // Aggiungi una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Imposta la proprietà RefreshDataOnOpeningFile
            pivotTable.RefreshDataOnOpeningFile = false;

            // Salva la cartella di lavoro
            workbook.Save("PivotTableRefreshDataOnOpeningFileDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


