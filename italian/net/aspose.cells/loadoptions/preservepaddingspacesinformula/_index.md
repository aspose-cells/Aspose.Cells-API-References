---
title: "LoadOptions.PreservePaddingSpacesInFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Indica se preservare quegli spazi e interruzioni di riga che sono inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/loadoptions/preservepaddingspacesinformula/
---
## LoadOptions.PreservePaddingSpacesInFormula property

Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. Il valore predefinito è false.

```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```

### Osservazioni

Dopo aver caricato la cartella di lavoro dal file modello con questa opzione, [`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) verrà impostato allo stesso valore di questa proprietà.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPreservePaddingSpacesInFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Abilita la conservazione degli spazi di riempimento nelle formule
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = true;
            
            // Accedi al primo foglio di lavoro e imposta una formula con spazi di riempimento
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            string formulaWithSpaces = "= IF(1 <>2, 2, 1)";
            cell.Formula = formulaWithSpaces;
            
            // Salva e ricarica la cartella di lavoro con l'opzione PreservePaddingSpacesInFormula
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx)
            {
                PreservePaddingSpacesInFormula = true
            };
            
            Workbook reloadedWorkbook = new Workbook(outputPath, loadOptions);
            Worksheet reloadedWorksheet = reloadedWorkbook.Worksheets[0];
            
            // Verifica che la formula abbia conservato gli spazi dopo il ricaricamento
            Console.WriteLine("Original formula: " + formulaWithSpaces);
            Console.WriteLine("Reloaded formula: " + reloadedWorksheet.Cells["A1"].Formula);
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


