---
title: "PivotTable.ShowReportFilterPageByIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Mostra tutte le pagine del filtro report in base all'indice di posizione nei PageFields"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showreportfilterpagebyindex/
---
## PivotTable.ShowReportFilterPageByIndex method

Mostra tutte le pagine di filtro del report in base all'indice di posizione nei PageFields.

```csharp
public void ShowReportFilterPageByIndex(int posIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| posIndex | Int32 | L'indice di posizione nei PageFields |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("PivotTable.xlsx");
            
            // Accedi al primo foglio di lavoro che contiene la tabella pivot
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Mostra le pagine del filtro report per indice (posizione) del campo pagina
            int pageFieldIndex = 0; // First page field
            pivotTable.ShowReportFilterPageByIndex(pageFieldIndex);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTable_ShowReportFilterPageByIndex_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


