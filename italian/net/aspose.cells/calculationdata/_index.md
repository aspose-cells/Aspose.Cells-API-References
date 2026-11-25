---
title: "Classe CalculationData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CalculationData. Rappresenta i dati necessari durante il calcolo di una funzione, come nome della funzione, parametri ...ecc"
type: docs
url: /it/net/aspose.cells/calculationdata/
---
## CalculationData class

Rappresenta i dati richiesti durante il calcolo di una funzione, come il nome della funzione, i parametri, ...ecc.

```csharp
public class CalculationData
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue/) { get; set; } | Ottiene o imposta il valore calcolato per questa funzione. |
| [Cell](../../aspose.cells/calculationdata/cell/) { get; } | Ottiene l'oggetto Cell in cui si trova la funzione. |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn/) { get; } | Ottiene l'indice della colonna della cella in cui si trova la funzione. |
| [CellRow](../../aspose.cells/calculationdata/cellrow/) { get; } | Ottiene l'indice della riga della cella in cui si trova la funzione. |
| [FunctionName](../../aspose.cells/calculationdata/functionname/) { get; } | Ottiene il nome della funzione da calcolare. |
| [ParamCount](../../aspose.cells/calculationdata/paramcount/) { get; } | Ottiene il conteggio dei parametri |
| [Workbook](../../aspose.cells/calculationdata/workbook/) { get; } | Ottiene l'oggetto Workbook in cui si trova la funzione. |
| [Worksheet](../../aspose.cells/calculationdata/worksheet/) { get; } | Ottiene l'oggetto Worksheet in cui si trova la funzione. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext/)(int) | Ottiene il testo letterale del parametro all'indice specificato. |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue/)(int) | Ottiene l'oggetto valore rappresentato del parametro a un dato indice. |
| [GetParamValueInArrayMode](../../aspose.cells/calculationdata/getparamvalueinarraymode/)(int, int, int) | Ottiene il valore/i del parametro a un dato indice. Se il parametro è una sorta di espressione che deve essere calcolata, verrà calcolato in modalità array. |

### Osservazioni

Tutti gli oggetti forniti da questa classe sono solo a scopo di \"lettura\". L'utente non dovrebbe modificare alcun dato nel Workbook durante il processo di calcolo della formula, altrimenti potrebbero verificarsi risultati inattesi o eccezioni.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCalculationDataDemo
    {
        public static void Run()
        {
            try
            {
                // Prepara un semplice workbook e worksheet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Name = "DemoSheet";

                // Inserisci alcuni valori che saranno usati come parametri in una funzione personalizzata
                sheet.Cells["A1"].PutValue(5);
                sheet.Cells["A2"].PutValue(10);

                // Imposta una formula che invoca la funzione personalizzata
                sheet.Cells["B1"].Formula = "=MYFUNC(A1, A2)";

                // Configura le opzioni di calcolo per utilizzare un motore personalizzato
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new DemoEngine();

                // Esegui il calcolo – il motore personalizzato riceverà un'istanza di CalculationData
                workbook.CalculateFormula(options);

                // Restituisci il risultato della funzione personalizzata
                Console.WriteLine("Custom function result (B1): " + sheet.Cells["B1"].Value);

                // Salva la cartella di lavoro per completezza
                workbook.Save("CalculationDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with CalculationData: {ex.Message}");
            }
        }

        // Motore di calcolo personalizzato che dimostra l'accesso ai membri di CalculationData
        private class DemoEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Assicurati che stiamo gestendo la funzione personalizzata prevista
                if (data.FunctionName != null &&
                    data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
                {
                    // Recupera i valori dei parametri (vengono restituiti come oggetti)
                    object param0 = data.GetParamValue(0);
                    object param1 = data.GetParamValue(1);

                    // Converti i parametri in double per il calcolo
                    double val0 = Convert.ToDouble(param0);
                    double val1 = Convert.ToDouble(param1);
                    double result = val0 + val1; // simple addition

                    // Assegna il risultato calcolato
                    data.CalculatedValue = result;

                    // Dimostra la lettura delle proprietà in sola lettura
                    Console.WriteLine("[Engine] FunctionName : " + data.FunctionName);
                    Console.WriteLine("[Engine] ParamCount   : " + data.ParamCount);
                    Console.WriteLine("[Engine] CellRow      : " + data.CellRow);
                    Console.WriteLine("[Engine] CellColumn   : " + data.CellColumn);
                }
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


