---
title: "PivotField.IsRepeatItemLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se ripetere le etichette del campo nella regione di riga o colonna. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

Indica se ripetere le etichette del campo nella regione riga o colonna. Il valore predefinito è false.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsRepeatItemLabelsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");

            // Accedi al foglio di lavoro contenente la tabella pivot
            Worksheet worksheet = workbook.Worksheets["Actual"];

            // Accedi alla tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];

            // Abilita la ripetizione delle etichette degli elementi per il primo campo di riga
            pivotTable.RowFields[0].IsRepeatItemLabels = true;

            // Abilita la ripetizione delle etichette degli elementi per il primo campo di colonna
            pivotTable.ColumnFields[0].IsRepeatItemLabels = true;

            // Salva la cartella di lavoro modificata
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


