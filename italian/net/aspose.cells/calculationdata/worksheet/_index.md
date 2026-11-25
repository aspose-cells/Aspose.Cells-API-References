---
title: "CalculationData.Worksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationData. Ottiene l'oggetto Worksheet in cui si trova la funzione"
type: docs
url: /it/net/aspose.cells/calculationdata/worksheet/
---
## CalculationData.Worksheet property

Ottiene l'oggetto Worksheet in cui si trova la funzione.

```csharp
public Worksheet Worksheet { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorksheetDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi alcuni dati per rendere l'esempio significativo
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Crea opzioni di calcolo con motore personalizzato
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new WorksheetDemoEngine();

                // Calcola le formule con opzioni
                workbook.CalculateFormula(options);

                // Visualizza il risultato
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Salva il risultato
                workbook.Save("WorksheetDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class WorksheetDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Accedi alla proprietà Worksheet in sola lettura
                Worksheet worksheet = data.Worksheet;
                Console.WriteLine($"Function is in worksheet: {worksheet.Name}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


