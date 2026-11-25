---
title: "AutoFitterOptions.AutoFitMergedCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFitterOptions. Indica se adattare automaticamente l'altezza della riga quando le celle sono unite in una riga. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/autofitteroptions/autofitmergedcells/
---
## AutoFitterOptions.AutoFitMergedCells property

Indica se adattare automaticamente l'altezza della riga quando le celle sono unite in una riga. Il valore predefinito è false.

```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà AutoFitterOptions.AutoFitMergedCellsType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2018. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio e unisci le celle
            worksheet.Cells["A1"].PutValue("This is a test of AutoFitMergedCells property");
            worksheet.Cells.Merge(0, 0, 3, 3); // Merge cells A1:C3

            // Crea AutoFitterOptions e imposta AutoFitMergedCells
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;

            // Adatta automaticamente le righe con celle unite
            worksheet.AutoFitRows(options);

            // Salva la cartella di lavoro
            workbook.Save("AutoFitMergedCellsExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


