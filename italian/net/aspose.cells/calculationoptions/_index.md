---
title: "Classe CalculationOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CalculationOptions. Rappresenta le opzioni per il calcolo"
type: docs
url: /it/net/aspose.cells/calculationoptions/
---
## CalculationOptions class

Rappresenta le opzioni per il calcolo.

```csharp
public class CalculationOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CalculationOptions](calculationoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CalcStackSize](../../aspose.cells/calculationoptions/calcstacksize/) { get; set; } | La dimensione dello stack per il calcolo ricorsivo delle celle. Il valore predefinito è 200. |
| [CalculationMonitor](../../aspose.cells/calculationoptions/calculationmonitor/) { get; set; } | Il monitor per l'utente per tracciare l'avanzamento del calcolo delle formule. |
| [CharacterEncoding](../../aspose.cells/calculationoptions/characterencoding/) { get; set; } | Specifica la codifica utilizzata per codificare/decodificare i caratteri durante il calcolo delle formule. Per funzioni come CHAR, CODE, il risultato calcolato dipende dalle impostazioni regionali e dal set di caratteri predefinito dell'ambiente. Con questa proprietà l'utente può specificare la codifica corretta da utilizzare per tali funzioni per ottenere il risultato previsto. |
| [CustomEngine](../../aspose.cells/calculationoptions/customengine/) { get; set; } | Il motore di calcolo delle formule personalizzato per estendere il motore di calcolo predefinito di Aspose.Cells. |
| [IgnoreError](../../aspose.cells/calculationoptions/ignoreerror/) { get; set; } | Indica se gli errori riscontrati durante il calcolo delle formule devono essere ignorati. L'errore può essere una funzione non supportata, collegamenti esterni, ecc. Il valore predefinito è true. |
| [LinkedDataSources](../../aspose.cells/calculationoptions/linkeddatasources/) { get; set; } | Specifica le origini dati per i collegamenti esterni utilizzati nelle formule. |
| [PrecisionStrategy](../../aspose.cells/calculationoptions/precisionstrategy/) { get; set; } | Specifica la strategia per l'elaborazione della precisione del calcolo. |
| [Recursive](../../aspose.cells/calculationoptions/recursive/) { get; set; } | Indica se calcolare ricorsivamente le celle dipendenti quando si calcola una cella che dipende da altre celle. Il valore predefinito è true. |
| [RefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/refreshdynamicarrayformula/) { get; set; } | Indica se le formule di array dinamici devono essere aggiornate prima di calcolare le formule. |
| [UserSpecifiedRefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/) { get; } | Indica se l'utente ha specificato esplicitamente il comportamento di aggiornamento delle formule di array dinamici prima di calcolare le formule specificate. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class CalculationOptionsDemo
    {
        public static void CalculationOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(10.555);
            worksheet.Cells["A2"].PutValue(20.6666);
            worksheet.Cells["A3"].PutValue(30.7777);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // Crea un'istanza di CalculationOptions
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                CalcStackSize = 200,
                PrecisionStrategy = CalculationPrecisionStrategy.Round,
                CharacterEncoding = Encoding.UTF8
            };

            // Facoltativamente, è possibile impostare un motore di calcolo personalizzato o un monitor
            // calcOptions.CustomEngine = new MyCustomEngine();
            // calcOptions.CalculationMonitor = new MyCalculationMonitor();

            // Calcola le formule nella cartella di lavoro con le opzioni specificate
            workbook.CalculateFormula(calcOptions);

            // Salva la cartella di lavoro
            workbook.Save("CalculationOptionsExample.xlsx");
            workbook.Save("CalculationOptionsExample.pdf");

        }
    }

    // Esempio di motore di calcolo personalizzato (se necessario)
    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Logica di calcolo personalizzata
            string funcName = data.FunctionName.ToUpper();
            if (funcName == "MYFUNC")
            {
                // Esempio di logica di funzione personalizzata
                int count = data.ParamCount;
                object result = null;
                for (int i = 0; i < count; i++)
                {
                    object paramValue = data.GetParamValue(i);
                    if (paramValue is ReferredArea)
                    {
                        ReferredArea ra = (ReferredArea)paramValue;
                        paramValue = ra.GetValue(0, 0);
                    }
                    // Elabora il parametro qui
                    // result = ...;
                }
                data.CalculatedValue = result;
            }
        }
    }

    // Esempio di monitor di calcolo personalizzato (se necessario)
    public class MyCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Logica prima del calcolo
            Console.WriteLine($"Before calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Logica dopo il calcolo
            Console.WriteLine($"After calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override bool OnCircular(System.Collections.IEnumerator circularCellsData)
        {
            // Gestisci riferimenti circolari
            Console.WriteLine("Circular reference detected.");
            return true; // Continue calculation
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


