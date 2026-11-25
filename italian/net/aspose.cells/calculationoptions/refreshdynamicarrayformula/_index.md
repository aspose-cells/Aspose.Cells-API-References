---
title: "CalculationOptions.RefreshDynamicArrayFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationOptions. Indica se le formule di array dinamici devono essere aggiornate prima di calcolare le formule"
type: docs
url: /it/net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

Indica se le formule di array dinamici devono essere aggiornate prima di calcolare le formule.

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### Osservazioni

Se questa proprietà è stata specificata esplicitamente, il valore specificato verrà utilizzato per determinare se aggiornare le formule di array dinamici. Altrimenti ([`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) è false), il valore predefinito dipende dal tipo di formule da calcolare: per il calcolo delle formule della cartella di lavoro, come [`CalculateFormula`](../../workbook/calculateformula/), questa proprietà sarà considerata true. Per altri casi, come [`Calculate`](../../cell/calculate/) o [`CalculateFormula`](../../worksheet/calculateformula/), questa proprietà sarà considerata false.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una formula di array dinamico per dimostrare la funzionalità
            worksheet.Cells["A1"].Value = 1;
            worksheet.Cells["A2"].Value = 2;
            worksheet.Cells["A3"].Value = 3;
            worksheet.Cells["B1"].Formula = "=A1:A3"; // Dynamic array formula

            // Crea un'istanza di CalculationOptions
            CalculationOptions options = new CalculationOptions();

            try
            {
                // Visualizza il valore predefinito di RefreshDynamicArrayFormula
                Console.WriteLine("Default RefreshDynamicArrayFormula value: " + options.RefreshDynamicArrayFormula);

                // Imposta la proprietà su true per aggiornare le formule di array dinamici
                options.RefreshDynamicArrayFormula = true;
                Console.WriteLine("After setting to true: " + options.RefreshDynamicArrayFormula);

                // Calcola le formule con le opzioni specificate
                workbook.CalculateFormula(options);

                // Visualizza il risultato calcolato
                Console.WriteLine("Dynamic array formula result: " + worksheet.Cells["B1"].Value);

                // Salva la cartella di lavoro
                workbook.Save("RefreshDynamicArrayFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


