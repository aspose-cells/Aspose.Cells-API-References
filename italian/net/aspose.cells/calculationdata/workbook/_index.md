---
title: "CalculationData.Workbook"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationData. Restituisce l'oggetto Workbook dove si trova la funzione"
type: docs
url: /it/net/aspose.cells/calculationdata/workbook/
---
## CalculationData.Workbook property

Ottiene l'oggetto Workbook in cui si trova la funzione.

```csharp
public Workbook Workbook { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio e formula
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].Formula = "=CUSTOMFUNC()";

            // Creare opzioni di calcolo e registrare un motore di calcolo personalizzato
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();

            // Attivare il calcolo con le opzioni per dimostrare l'uso della proprietà Workbook
            workbook.CalculateFormula(options);

            // Visualizzare il risultato del calcolo
            Console.WriteLine("Calculated value in B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("Modified value in C1: " + worksheet.Cells["C1"].Value);

            // Salva il risultato
            workbook.Save("PropertyWorkbookDemo.xlsx");
        }

        private class CustomCalcEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "CUSTOMFUNC")
                {
                    // Accedere alla proprietà Workbook da CalculationData
                    Workbook currentWorkbook = data.Workbook;
                    Worksheet currentSheet = currentWorkbook.Worksheets[0];

                    // Dimostrare l'uso della cartella di lavoro per manipolare i dati
                    double inputValue = (double)currentSheet.Cells["A1"].Value;
                    currentSheet.Cells["C1"].PutValue(inputValue * 2);

                    // Impostare il risultato calcolato
                    data.CalculatedValue = inputValue * 3;
                }
            }
        }
    }
}
```

### Vedi anche

* class [Workbook](../../workbook/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


