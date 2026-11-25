---
title: "CalculationOptions.IgnoreError"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationOptions. Indica se gli errori riscontrati durante il calcolo delle formule devono essere ignorati. L'errore può essere una funzione non supportata, collegamenti esterni, ecc. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

Indica se gli errori riscontrati durante il calcolo delle formule devono essere ignorati. L'errore può essere una funzione non supportata, collegamenti esterni, ecc. Il valore predefinito è true.

```csharp
public bool IgnoreError { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un intervallo denominato che non esiste per dimostrare la gestione degli errori
            worksheet.Cells["A1"].Formula = "=NONEXISTENTNAME()";
            
            // Calcola con IgnoreError = false (genererà un errore)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = false });
                Console.WriteLine("Calculation completed without ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (expected): " + ex.Message);
            }

            // Calcola con IgnoreError = true (sopprimerà l'errore)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = true });
                Console.WriteLine("Calculation completed while ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (unexpected): " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


