---
title: "LoadOptions.CheckDataValid"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Verifica se i dati sono validi nel file modello"
type: docs
url: /it/net/aspose.cells/loadoptions/checkdatavalid/
---
## LoadOptions.CheckDataValid property

Verifica se i dati sono validi nel file modello.

```csharp
public bool CheckDataValid { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckDataValidDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento con CheckDataValid impostato su false
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CheckDataValid = false;

            // Carica la cartella di lavoro con queste opzioni
            Workbook workbook = new Workbook("example.xlsx", options);

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una convalida dei dati per dimostrazione
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Imposta l'intervallo di convalida
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 10;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


