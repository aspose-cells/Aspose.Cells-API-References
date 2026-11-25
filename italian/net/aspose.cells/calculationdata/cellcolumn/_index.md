---
title: "CalculationData.CellColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationData. Ottiene l'indice di colonna della cella in cui si trova la funzione"
type: docs
url: /it/net/aspose.cells/calculationdata/cellcolumn/
---
## CalculationData.CellColumn property

Ottiene l'indice della colonna della cella in cui si trova la funzione.

```csharp
public int CellColumn { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellColumnDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi dati di esempio con formule in colonne diverse
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["B1"].PutValue(20);
                worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

                // Crea opzioni di calcolo con motore personalizzato
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellColumnDemoEngine();

                // Calcola le formule
                workbook.CalculateFormula(options);

                // Visualizza il risultato calcolato
                Console.WriteLine("Calculated value in C1: " + worksheet.Cells["C1"].Value);

                // Salva il risultato
                workbook.Save("CellColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellColumnDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data != null)
            {
                // Accedi alla proprietà CellColumn in sola lettura
                int columnIndex = data.CellColumn;
                Console.WriteLine($"Function is in column index: {columnIndex}");

                // Dimostra l'uso delle informazioni di colonna
                if (data.FunctionName == "SUM")
                {
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
}
```

### Vedi anche

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


