---
title: "PivotTable.ShowReportFilterPage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Mostra tutte le pagine di filtro del report in base al PivotField; il PivotField deve trovarsi nei PageFields"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showreportfilterpage/
---
## PivotTable.ShowReportFilterPage method

Mostra tutte le pagine di filtro del report in base a PivotField, il PivotField deve trovarsi nei PageFields.

```csharp
public void ShowReportFilterPage(PivotField pageField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageField | PivotField | L'oggetto PivotField |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageWithPivotFieldDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("source.xlsx");
            
            // Accedi al primo foglio di lavoro e alla tabella pivot
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Mostra le pagine di filtro del report per ogni campo di pagina
            foreach (PivotField pageField in pivotTable.PageFields)
            {
                pivotTable.ShowReportFilterPage(pageField);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


