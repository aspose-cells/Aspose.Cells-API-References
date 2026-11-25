---
title: "Worksheet.CalculateFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Calcola una formula"
type: docs
url: /it/net/aspose.cells/worksheet/calculateformula/
---
## CalculateFormula(string) {#calculateformula}

Calcola una formula.

```csharp
public object CalculateFormula(string formula)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | Formula da calcolare. |

### Valore di ritorno

Risultato della formula calcolata.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Worksheet sheet = wb.Worksheets[0];

            // Dimostra la conversione di numeri di base
            string formula = "=NUMBERVALUE(\"1.234\")";
            Console.WriteLine("NUMBERVALUE(\"1.234\") = " + sheet.CalculateFormula(formula));

            // Dimostra la conversione di valuta
            formula = "=NUMBERVALUE(\"$1,234.56\")";
            Console.WriteLine("NUMBERVALUE(\"$1,234.56\") = " + sheet.CalculateFormula(formula));

            // Dimostra la conversione di tempo
            formula = "=NUMBERVALUE(\"0:25\")";
            Console.WriteLine("NUMBERVALUE(\"0:25\") = " + sheet.CalculateFormula(formula));

            // Dimostra la conversione di data
            formula = "=NUMBERVALUE(\"07/26/2023\")";
            Console.WriteLine("NUMBERVALUE(\"07/26/2023\") = " + sheet.CalculateFormula(formula));

            // Dimostra il caso di errore
            formula = "=NUMBERVALUE(\"invalid\")";
            Console.WriteLine("NUMBERVALUE(\"invalid\") = " + sheet.CalculateFormula(formula));
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, CalculationOptions) {#calculateformula_1}

Calcola direttamente un'espressione di formula.

```csharp
public object CalculateFormula(string formula, CalculationOptions opts)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | Formula da calcolare. |
| opts | CalculationOptions | Opzioni per il calcolo della formula |

### Valore di ritorno

Risultato calcolato della formula fornita. L'oggetto restituito può essere di possibili tipi di [`Value`](../../cell/value/), o ReferredArea.

### Osservazioni

La formula verrà calcolata proprio come se fosse impostata nella cella A1. E la formula sarà considerata una formula normale. Se hai bisogno che la formula venga calcolata come formula matrice e di ottenere un array per il risultato calcolato, utilizza [`CalculateArrayFormula`](../calculatearrayformula/) invece.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Crea un motore di calcolo personalizzato
            CustomEngine customEngine = new CustomEngine();
            
            // Calcola la formula utilizzando il motore personalizzato
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };
            
            object result = worksheet.CalculateFormula("=SUM(A1:A3)", options);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object value = data.GetParamValue(i);
                    if (value is double)
                    {
                        sum += (double)value;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### Vedi anche

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) {#calculateformula_2}

Calcola direttamente un'espressione di formula.

```csharp
public object CalculateFormula(string formula, FormulaParseOptions pOpts, CalculationOptions cOpts, 
    int baseCellRow, int baseCellColumn, CalculationData calculationData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | Formula da calcolare. |
| pOpts | FormulaParseOptions | Opzioni per l'analisi della formula. |
| cOpts | CalculationOptions | Opzioni per il calcolo della formula. |
| baseCellRow | Int32 | L'indice di riga della cella di base. |
| baseCellColumn | Int32 | L'indice di colonna della cella di base. |
| calculationData | CalculationData | I dati di calcolo. Sono usati per la situazione in cui l'utente deve calcolare alcune formule statiche quando implementa un motore di calcolo personalizzato. Per questo tipo di situazione, l'utente deve specificarli con i dati di calcolo forniti per [`Calculate`](../../abstractcalculationengine/calculate/). |

### Valore di ritorno

Risultato calcolato della formula fornita. L'oggetto restituito può essere di possibili tipi di [`Value`](../../cell/value/), o ReferredArea.

### Osservazioni

La formula verrà calcolata proprio come se fosse impostata nella cella di base specificata. E la formula sarà trattata come una formula normale. Se hai bisogno che la formula venga calcolata come formula matriciale e di ottenere un array per il risultato calcolato, utilizza [`CalculateArrayFormula`](../calculatearrayformula/) invece.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringFormulaParseOptCalculati169472Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola dati di esempio
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C1"].PutValue(2);
            worksheet.Cells["C2"].PutValue(4);

            // Definisci le opzioni di calcolo
            CalculationOptions calculationOptions = new CalculationOptions();
            
            // Definisci le opzioni di analisi della formula
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions();
            
            // Calcola la formula con tutti i parametri
            object result = worksheet.CalculateFormula(
                "=SUM(B1:B2, C1:C2)",  // formula
                formulaParseOptions,   // parse options
                calculationOptions,    // calculation options
                0,                     // base cell row
                0,                     // base cell column
                null                   // calculation data
            );

            // Restituisci il risultato
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Vedi anche

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions, bool) {#calculateformula_3}

Calcola tutte le formule in questo foglio di lavoro.

```csharp
public void CalculateFormula(CalculationOptions options, bool recursive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | CalculationOptions | Opzioni per il calcolo |
| ricorsivo | Booleano | True indica che se le celle del foglio di lavoro dipendono dalle celle di altri fogli di lavoro, le celle dipendenti negli altri fogli verranno calcolate anch'esse. False indica che tutte le formule nel foglio di lavoro sono state calcolate e i valori sono corretti. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithCalculationOptionsBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio e formule
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue("=SUM(A1:A3)");
            
            // Crea le opzioni di calcolo
            CalculationOptions options = new CalculationOptions();
            options.Recursive = true;
            options.IgnoreError = false;
            
            // Calcola la formula con opzioni e forzare il calcolo completo
            worksheet.CalculateFormula(options, true);
            
            // Restituisci il risultato calcolato
            Console.WriteLine("Calculated value: " + worksheet.Cells["B1"].StringValue);
        }
    }
}
```

### Vedi anche

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


