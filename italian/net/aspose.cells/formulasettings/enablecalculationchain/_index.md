---
title: "FormulaSettings.EnableCalculationChain"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. Indica se abilitare la catena di calcolo per le formule. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

Indica se abilitare la catena di calcolo per le formule. Il valore predefinito è false.

```csharp
public bool EnableCalculationChain { get; set; }
```

### Osservazioni

Quando nella cartella di lavoro ci sono molte formule e l'utente deve calcolarle ripetutamente modificando solo una piccola parte di esse, abilitare la catena di calcolo può migliorare le prestazioni. D'altra parte, se la catena è abilitata, mantenere il modello della catena richiede più memoria e comporta un leggero aumento del tempo CPU per alcune operazioni, come la modifica del valore di una cella o delle formule. Dopo aver cambiato questa proprietà da false a true, la catena di calcolo verrà analizzata e costruita al momento del primo calcolo della cartella di lavoro, quindi il tempo richiesto per il primo calcolo potrebbe essere superiore a quello di un calcolo normale senza catena.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyEnableCalculationChainDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi formule di esempio
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";
            
            // Disabilita la catena di calcolo
            workbook.Settings.FormulaSettings.EnableCalculationChain = false;
            
            // Calcola le formule
            workbook.CalculateFormula();
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with calculation chain disabled.");
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


