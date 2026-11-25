---
title: "Worksheet.CalculateArrayFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Calcola una formula come formula array"
type: docs
url: /it/net/aspose.cells/worksheet/calculatearrayformula/
---
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}

Calcola una formula come formula di matrice.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | Formula da calcolare. |
| opts | CalculationOptions | Opzioni per il calcolo della formula |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Definisci una formula array
            string arrayFormula = "=SUM(A1:B3)";
            
            // Calcola la formula array con le opzioni di calcolo
            object[][] result = worksheet.CalculateArrayFormula(arrayFormula, new CalculationOptions());
            
            // Restituisci il risultato
            Console.WriteLine("Result of array formula calculation: " + result[0][0]);
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

## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}

Calcola una formula come formula di matrice.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount, 
    int maxColumnCount)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | Formula da calcolare. |
| opts | CalculationOptions | Opzioni per il calcolo della formula |
| maxRowCount | Int32 | il numero massimo di righe dei dati risultanti. Se è non positivo o maggiore del numero reale di righe, verrà usato il numero reale di righe. |
| maxColumnCount | Int32 | il numero massimo di colonne dei dati risultanti. Se è non positivo o maggiore del numero reale di righe, verrà usato il numero reale di colonne. |

### Valore di ritorno

Risultato della formula calcolata.

### Osservazioni

La formula verrà considerata come formula array dinamica per calcolare la dimensione e il risultato. La dimensione massima specificata dall'utente viene utilizzata nei casi in cui il risultato calcolato è un set di dati di grandi dimensioni (ad esempio, il risultato calcolato può corrispondere a un'intera riga o colonna) ma l'utente non necessita di un array così grande secondo i requisiti aziendali o per considerazioni di prestazioni.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsInt32IDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Esempio 1: Calcolo semplice di formula array
            string formula = "=ISBLANK(IF(TRUE,B2:B5))";
            CalculationOptions options = new CalculationOptions();
            object[][] result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of ISBLANK(IF(TRUE,B2:B5)): " + result[0][0]);

            // Esempio 2: Formula array con intervallo dinamico
            formula = "=LEN(IF({1;2;3;4},B2:B5))";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of LEN(IF({1;2;3;4},B2:B5)): " + result[0][0]);

            // Esempio 3: Formula array con funzione MATCH
            // Imposta alcuni dati di test
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(10);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["C3"].PutValue(2);
            sheet.Cells["D2"].PutValue(0);
            sheet.Cells["D3"].PutValue(0);

            formula = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of MATCH formula: " + result[0][0]);
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

## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}

Calcola una formula come formula di matrice.

```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts, 
    CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, 
    int maxColumnCount, CalculationData calculationData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | Formula da calcolare. |
| pOpts | FormulaParseOptions | Opzioni per l'analisi della formula |
| cOpts | CalculationOptions | Opzioni per il calcolo della formula |
| baseCellRow | Int32 | L'indice di riga della cella di base. |
| baseCellColumn | Int32 | L'indice di colonna della cella di base. |
| maxRowCount | Int32 | Il numero massimo di righe dei dati risultanti. Se è non positivo o maggiore del numero reale di righe, verrà utilizzato il numero reale di righe. |
| maxColumnCount | Int32 | Il numero massimo di colonne dei dati risultanti. Se è non positivo o maggiore del numero reale di colonne, verrà utilizzato il numero reale di colonne. |
| calculationData | CalculationData | I dati di calcolo. Sono usati per la situazione in cui l'utente deve calcolare alcune formule statiche quando implementa un motore di calcolo personalizzato. Per questo tipo di situazione, l'utente deve specificarli con i dati di calcolo forniti per [`Calculate`](../../abstractcalculationengine/calculate/). |

### Valore di ritorno

Risultato della formula calcolata.

### Osservazioni

La formula verrà considerata come formula array dinamica per calcolare la dimensione e il risultato. La dimensione massima specificata dall'utente viene utilizzata nei casi in cui il risultato calcolato è un set di dati di grandi dimensioni (ad esempio, il risultato calcolato può corrispondere a un'intera riga o colonna) ma l'utente non necessita di un array così grande secondo i requisiti aziendali o per considerazioni di prestazioni.

### Vedi anche

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


