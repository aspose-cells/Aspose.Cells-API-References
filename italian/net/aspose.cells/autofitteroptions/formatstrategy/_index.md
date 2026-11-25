---
title: "AutoFitterOptions.FormatStrategy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFitterOptions. Ottiene e imposta la strategia di formattazione"
type: docs
url: /it/net/aspose.cells/autofitteroptions/formatstrategy/
---
## AutoFitterOptions.FormatStrategy property

Ottiene e imposta la strategia di formattazione.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Osservazioni

Il valore predefinito è CellStyle per le prestazioni.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta dati di esempio e avvolgi il testo
            worksheet.Cells["A1"].PutValue("Sample text for FormatStrategy demo");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Crea AutoFitterOptions con FormatStrategy
            AutoFitterOptions options = new AutoFitterOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine
            };

            // Applica l'adattamento automatico con le opzioni specificate
            worksheet.AutoFitRows(options);

            // Salva il risultato
            workbook.Save("FormatStrategyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


