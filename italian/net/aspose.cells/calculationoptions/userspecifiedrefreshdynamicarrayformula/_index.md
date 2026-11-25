---
title: "CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationOptions. Indica se l'utente ha specificato esplicitamente il comportamento di aggiornamento delle formule di array dinamici prima di calcolare le formule specificate"
type: docs
url: /it/net/aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/
---
## CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property

Indica se l'utente ha specificato esplicitamente il comportamento di aggiornamento delle formule di array dinamici prima di calcolare le formule specificate.

```csharp
public bool UserSpecifiedRefreshDynamicArrayFormula { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyUserSpecifiedRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea un'istanza di CalculationOptions
                CalculationOptions options = new CalculationOptions();

                // Visualizza il valore corrente della proprietà UserSpecifiedRefreshDynamicArrayFormula
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula value: " +
                    options.UserSpecifiedRefreshDynamicArrayFormula);

                // Mostra come la proprietà influisce sul comportamento
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula has been demonstrated");

                // Salva il risultato
                workbook.Save("UserSpecifiedRefreshDynamicArrayFormulaDemo.xlsx");
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


