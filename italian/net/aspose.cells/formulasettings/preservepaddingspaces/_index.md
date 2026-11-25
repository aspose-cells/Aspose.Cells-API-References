---
title: "FormulaSettings.PreservePaddingSpaces"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

Indica se conservare gli spazi e le interruzioni di riga inseriti tra i token delle formule durante il recupero e l'impostazione delle formule. Il valore predefinito è false.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### Osservazioni

In genere quegli spazi e interruzioni di riga servono solo a scopo visivo; preservarli o meno non influisce sul risultato calcolato. Per motivi di prestazioni, se non vi è alcuna esigenza speciale, è preferibile non preservarli durante l'elaborazione delle formule.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPreservePaddingSpacesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la formula con spazi di riempimento
            string formulaWithSpaces = "=SUM( IF( A1:A5 > 10, B1:B5, 0 ) )";
            worksheet.Cells["C1"].Formula = formulaWithSpaces;
            
            // Comportamento predefinito (PreservePaddingSpaces è true)
            Console.WriteLine("Formula with spaces preserved: " + worksheet.Cells["C1"].Formula);
            
            // Modifica l'impostazione per rimuovere gli spazi di riempimento
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = false;
            worksheet.Cells["C2"].Formula = formulaWithSpaces;
            
            Console.WriteLine("Formula with spaces removed: " + worksheet.Cells["C2"].Formula);
            
            // Salva la cartella di lavoro
            workbook.Save("FormulaSpacesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


