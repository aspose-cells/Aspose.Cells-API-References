---
title: "Cell.SetDynamicArrayFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Imposta la formula di array dinamico e fa sì che la formula si espanda nelle celle vicine, se possibile"
type: docs
url: /it/net/aspose.cells/cell/setdynamicarrayformula/
---
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}

Imposta una formula di matrice dinamica e fa sì che la formula si espanda nelle celle vicine, se possibile.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    bool calculateValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | String | l'espressione della formula |
| opzioni | FormulaParseOptions | opzioni per analizzare la formula. L'opzione "Parse" verrà ignorata e la formula verrà sempre analizzata immediatamente |
| calculateValue | Booleano | se calcolare questa formula di array dinamico per quelle celle nell'intervallo di spill. |

### Valore di ritorno

l'intervallo in cui la formula dovrebbe spillare.

### Osservazioni

l'intervallo restituito potrebbe non essere lo stesso di quello effettivo in cui questa formula di array dinamico spillerebbe. Se ci sono celle non vuote nell'intervallo, la formula verrà impostata solo per la cella corrente e contrassegnata come "#SPILL!". Ma per questo tipo di situazione restituiamo comunque l'intero intervallo in cui questa formula dovrebbe spillare.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsBooleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Imposta la formula di array dinamico nella cella A1
            Cell cell1 = cells["A1"];
            cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);

            // Imposta il valore in B2 che influenzerà la formula SEQUENCE
            cells["B2"].PutValue(3);

            // Calcola le formule e aggiorna gli array dinamici
            wb.CalculateFormula();
            wb.RefreshDynamicArrayFormulas(false);

            // Restituisci i risultati dall'intervallo spillato
            Console.WriteLine("Dynamic array results:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine(cells[0, i].Value);
            }
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}

Imposta una formula di matrice dinamica e fa sì che la formula si espanda nelle celle vicine, se possibile.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | String | l'espressione della formula |
| opzioni | FormulaParseOptions | opzioni per analizzare la formula. L'opzione "Parse" verrà ignorata e la formula verrà sempre analizzata immediatamente |
| valori | Object[][] | valori (risultati calcolati) per quelle celle con la formula di array dinamico fornita |
| calculateRange | Booleano | Se calcolare l'intervallo spillato per questa formula di array dinamico. Se il parametro "values" non è nullo e questa flag è falsa, l'altezza dell'intervallo spillato sarà values.Length e la larghezza sarà values[0].Length. |
| calculateValue | Booleano | se calcolare questa formula di array dinamico per quelle celle nell'intervallo spillato quando "values" è nullo o l'elemento corrispondente in "values" per una cella è nullo. |

### Valore di ritorno

l'intervallo in cui la formula dovrebbe spillare.

### Osservazioni

l'intervallo restituito potrebbe non essere lo stesso di quello effettivo in cui questa formula di array dinamico spillerebbe. Se ci sono celle non vuote nell'intervallo, la formula verrà impostata solo per la cella corrente e contrassegnata come "#SPILL!". Ma per questo tipo di situazione restituiamo comunque l'intero intervallo in cui questa formula dovrebbe spillare.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue(10);
            cell = cells["A2"];
            cell.PutValue(20);
            cell = cells["B1"];
            cell.PutValue(60);
            cell = cells["B2"];
            cell.PutValue(80);

            // Ottieni la cella C1 dove verrà impostata la formula di array dinamico
            cell = worksheet.Cells["C1"];

            // Definisci la formula di array dinamico
            string formula = "=A1:B2 * 2";
            
            // Crea le opzioni di analisi della formula
            FormulaParseOptions options = new FormulaParseOptions
            {
                Parse = true // Enable formula parsing
            };

            // Prepara i valori per popolare le celle risultato della formula
            object[][] values = new object[2][];
            values[0] = new object[] { 2, 4 };
            values[1] = new object[] { 6, 8 };

            try
            {
                // Imposta la formula di array dinamico con valori pre-calcolati
                CellArea result = cell.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange: false,  // Use values array dimensions for spill range
                    calculateValue: false  // Use provided values instead of calculating
                );

                Console.WriteLine($"Dynamic array formula set. Affected range: Rows {result.StartRow}-{result.EndRow}, Columns {result.StartColumn}-{result.EndColumn}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula: {ex.Message}");
            }

            // Salva la cartella di lavoro con le modifiche
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) {#setdynamicarrayformula_2}

Imposta una formula di matrice dinamica e fa sì che la formula si espanda nelle celle vicine, se possibile.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | String | l'espressione della formula |
| opzioni | FormulaParseOptions | opzioni per analizzare la formula. L'opzione "Parse" verrà ignorata e la formula verrà sempre analizzata immediatamente |
| valori | Object[][] | valori (risultati calcolati) per quelle celle con la formula di array dinamico fornita |
| calculateRange | Booleano | Se calcolare l'intervallo spillato per questa formula di array dinamico. Se il parametro "values" non è nullo e questa flag è falsa, l'altezza dell'intervallo spillato sarà values.Length e la larghezza sarà values[0].Length. |
| calculateValue | Booleano | se calcolare questa formula di array dinamico per quelle celle nell'intervallo spillato quando "values" è nullo o l'elemento corrispondente in "values" per una cella è nullo. |
| copts | CalculationOptions | Le opzioni per calcolare la formula. Comunemente, per motivi di prestazioni, la proprietà [`Recursive`](../../calculationoptions/recursive/) dovrebbe essere false. |

### Valore di ritorno

l'intervallo in cui la formula dovrebbe spillare.

### Osservazioni

l'intervallo restituito potrebbe non essere lo stesso di quello effettivo in cui questa formula di array dinamico spillerebbe. Se ci sono celle non vuote nell'intervallo, la formula verrà impostata solo per la cella corrente e contrassegnata come "#SPILL!". Ma per questo tipo di situazione restituiamo comunque l'intero intervallo in cui questa formula dovrebbe spillare.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio nelle celle A2:B5
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B3"].PutValue(55);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["B5"].PutValue(70);

            // Ottieni la cella obiettivo D1
            Cell cellD1 = worksheet.Cells["D1"];

            try
            {
                // Prepara i parametri per SetDynamicArrayFormula
                string formula = "=FILTER(A2:A5, B2:B5>50)";
                FormulaParseOptions options = new FormulaParseOptions { Parse = true };
                object[][] values = new object[2][] { new object[] { 10 }, new object[] { 40 } };
                bool calculateRange = true;
                bool calculateValue = true;
                CalculationOptions calcOptions = new CalculationOptions { Recursive = true };

                // Chiama SetDynamicArrayFormula con parametri specifici
                CellArea spillRange = cellD1.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange,
                    calculateValue,
                    calcOptions
                );

                Console.WriteLine($"Dynamic array formula set successfully. Spill range: {spillRange}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


