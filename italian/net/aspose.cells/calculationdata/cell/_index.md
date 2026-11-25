---
title: "CalculationData.Cell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationData. Restituisce l'oggetto Cell dove si trova la funzione"
type: docs
url: /it/net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

Ottiene l'oggetto Cell in cui si trova la funzione.

```csharp
public Cell Cell { get; }
```

### Osservazioni

Quando si calcola una formula senza impostarla in una cella, ad esempio tramite [`CalculateFormula`](../../worksheet/calculateformula/), la formula verrà calcolata come se fosse stata impostata nella cella A1, quindi sia [`CellRow`](../cellrow/) sia [`CellColumn`](../cellcolumn/) saranno 0. Tuttavia, la cella A1 nel foglio di lavoro potrebbe non essere stata istanziata. Perciò, in questo tipo di situazione, questa proprietà sarà null.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellDemo
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
                options.CustomEngine = new CellDemoEngine();

                // Calcola le formule con opzioni
                workbook.CalculateFormula(options);

                // Visualizza il risultato
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Salva il risultato
                workbook.Save("CellDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Accedere alla proprietà Cell di sola lettura
                Cell cell = data.Cell;
                Console.WriteLine($"Function is in cell: {cell.Name}");
                Console.WriteLine($"Cell value: {cell.StringValue}");
                Console.WriteLine($"Cell row: {cell.Row}, column: {cell.Column}");

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

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


