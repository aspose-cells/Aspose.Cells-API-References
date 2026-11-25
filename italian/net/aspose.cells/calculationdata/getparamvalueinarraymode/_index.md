---
title: "CalculationData.GetParamValueInArrayMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CalculationData. Ottiene i valori del parametro a un indice specificato. Se il parametro è una sorta di espressione che necessita di essere calcolata, verrà calcolato in modalità array"
type: docs
url: /it/net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

Ottiene il valore/i del parametro a un dato indice. Se il parametro è una sorta di espressione che deve essere calcolata, verrà calcolato in modalità array.

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice del parametro (base 0) |
| maxRowCount | Int32 | Il limite di conteggio delle righe per l'array restituito. Se è non positivo o maggiore del conteggio reale delle righe, verrà utilizzato il conteggio reale delle righe. |
| maxColumnCount | Int32 | Il limite di conteggio delle colonne per l'array restituito. Se è non positivo o maggiore del conteggio reale delle righe, verrà utilizzato il conteggio reale delle colonne. |

### Valore di ritorno

Un array che contiene tutti gli elementi rappresentati dal parametro specificato.

### Osservazioni

Per un'espressione che deve essere calcolata, prendendo A:A+B:B come esempio: in modalità valore verrà calcolata in un singolo valore in base alla cella corrente. Ma in modalità array, tutti i valori di A1+B1, A2+B2, A3+B3, ... verranno calcolati e usati per costruire l'array restituito. E per questo tipo di situazione è meglio specificare il limite per il conteggio di righe/colonne (ad esempio secondo [`MaxDataRow`](../../cells/maxdatarow/) e [`MaxDataColumn`](../../cells/maxdatacolumn/)), altrimenti il grande array restituito può aumentare il consumo di memoria con una grande quantità di dati inutili.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il contesto
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Formula = "=SUM(A1:C3)";

            try
            {
                // Crea opzioni di calcolo con motore personalizzato
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ArrayModeCalculationEngine();
                workbook.CalculateFormula(options);

                Console.WriteLine("GetParamValueInArrayMode method called successfully");
                workbook.Save("GetParamValueInArrayModeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetParamValueInArrayMode: {ex.Message}");
            }
        }

        private class ArrayModeCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "SUM")
                {
                    // Chiama GetParamValueInArrayMode con parametri realistici
                    object[][] paramArray = data.GetParamValueInArrayMode(0, 5, 3);

                    Console.WriteLine($"Parameter array dimensions: {paramArray.Length} rows");
                    if (paramArray.Length > 0)
                    {
                        Console.WriteLine($"First row has {paramArray[0].Length} columns");
                    }
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


