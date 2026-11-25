---
title: "LoadOptions.ParsingPivotCachedRecords"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Indica se analizzare i record pivot memorizzati nella cache durante il caricamento del file. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/loadoptions/parsingpivotcachedrecords/
---
## LoadOptions.ParsingPivotCachedRecords property

Indica se analizzare i record della cache pivot durante il caricamento del file. Il valore predefinito è false.

```csharp
public bool ParsingPivotCachedRecords { get; set; }
```

### Osservazioni

Si applica solo ai file Excel Xlsx, Xltx, Xltm, Xlsm e xlsb

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingPivotCachedRecordsDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            
            // Abilita l'analisi dei record pivot memorizzati nella cache
            loadOptions.ParsingPivotCachedRecords = true;
            
            // Carica la cartella di lavoro con le opzioni
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "PivotData";
            
            // Crea una tabella pivot (dimostrando che la proprietà è impostata)
            int pivotIndex = worksheet.PivotTables.Add("A1:C10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


