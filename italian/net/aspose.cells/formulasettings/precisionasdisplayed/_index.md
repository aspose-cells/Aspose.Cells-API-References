---
title: "FormulaSettings.PrecisionAsDisplayed"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. Indica se la precisione del risultato calcolato deve essere impostata come visualizzata durante il calcolo delle formule"
type: docs
url: /it/net/aspose.cells/formulasettings/precisionasdisplayed/
---
## FormulaSettings.PrecisionAsDisplayed property

Indica se la precisione del risultato calcolato deve essere impostata così come viene visualizzata durante il calcolo delle formule.

```csharp
public bool PrecisionAsDisplayed { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPrecisionAsDisplayedDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Imposta PrecisionAsDisplayed su true
            workbook.Settings.FormulaSettings.PrecisionAsDisplayed = true;
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Imposta il formato di visualizzazione per la cella A1 per mostrare 2 cifre decimali
            cells["A1"].PutValue(1.23456);
            Style style = cells["A1"].GetStyle();
            style.Number = 2; // Format: 0.00
            cells["A1"].SetStyle(style);
            
            // Imposta la formula nella cella B1 che fa riferimento a A1
            cells["B1"].Formula = "=A1";
            
            // Calcola le formule con PrecisionAsDisplayed abilitato
            workbook.CalculateFormula();
            
            // Restituisci i risultati
            Console.WriteLine("A1 Display Value: " + cells["A1"].StringValue); // Shows 1.23
            Console.WriteLine("B1 Calculated Value: " + cells["B1"].Value);   // Should be 1.23 due to PrecisionAsDisplayed
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


