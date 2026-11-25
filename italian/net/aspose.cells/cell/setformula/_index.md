---
title: "Cell.SetFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Imposta la formula e il valore (risultato calcolato) della formula"
type: docs
url: /it/net/aspose.cells/cell/setformula/
---
## SetFormula(string, object) {#setformula_3}

Imposta la formula e il valore (risultato calcolato) della formula.

```csharp
public void SetFormula(string formula, object value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | La formula. |
| valore | Object | Il valore (risultato calcolato) della formula. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringObjectDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta la formula con parametri stringa e oggetto
            cells["A1"].SetFormula("=SUM(1,2)", 4); // Will display 4 until calculation
            cells["A2"].SetFormula("=AVERAGE(5,10)", 7.5); // Will display 7.5 until calculation

            // Visualizza i valori prima del calcolo
            Console.WriteLine("Before Calculation:");
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);

            // Calcola le formule
            workbook.CalculateFormula();

            // Visualizza i valori dopo il calcolo
            Console.WriteLine("\nAfter Calculation:");
            Console.WriteLine("A1: " + cells["A1"].IntValue); // Should show 3
            Console.WriteLine("A2: " + cells["A2"].DoubleValue); // Should show 7.5
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions) {#setformula}

Imposta la formula e il valore (risultato calcolato) della formula.

```csharp
public void SetFormula(string formula, FormulaParseOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | La formula. |
| opzioni | FormulaParseOptions | Opzioni per l'analisi della formula. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni una cella specifica (B2 in questo caso)
            Cell cell = worksheet.Cells["B2"];
            
            // Imposta alcuni valori iniziali per la dimostrazione
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            
            // Esempio 1: Imposta una formula semplice con le opzioni di parsing predefinite
            cell.SetFormula("=SUM(A1:A2)", new FormulaParseOptions());
            Console.WriteLine("Formula with default options: " + cell.Formula);
            
            // Esempio 2: Imposta la formula con stile R1C1 usando FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            
            cell.SetFormula("=SUM(R[-1]C[-1]:R[0]C[-1])", options);
            Console.WriteLine("Formula with R1C1 style: " + cell.Formula);
            
            // Esempio 3: Imposta la formula con opzioni di parsing che preservano il formato R1C1
            options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            cell.SetFormula("=R1C1+R2C2", options);
            Console.WriteLine("Formula preserved as R1C1: " + cell.Formula);
            
            // Calcola la cartella di lavoro per vedere i risultati
            workbook.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.Value);
        }
    }
}
```

### Vedi anche

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, bool, bool, object) {#setformula_2}

Imposta la formula e il valore della formula.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetFormula(string formula, bool isR1C1, bool isLocal, object value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | La formula. |
| isR1C1 | Booleano | Indica se la formula è una formula R1C1. |
| isLocal | Booleano | Se la formula è formattata secondo la locale. |
| valore | Object | Il valore della formula. |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.SetFormula(string,FormulaParseOptions,object). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2019. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetFormulaWithStringBooleanBooleanObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);

            // Ottieni la cella di destinazione dove imposteremo la formula
            Cell cell = worksheet.Cells["C1"];

            try
            {
                // Imposta una formula con tutti i parametri
                // Parametri: stringa formula, isR1C1, isLocal, valore
                cell.SetFormula("=SUM(A1:B2)", false, false, null);

                // Calcola la formula
                workbook.CalculateFormula();

                // Visualizza il risultato
                Console.WriteLine($"Formula set successfully. Result: {cell.Value}");

                // Salva la cartella di lavoro
                workbook.Save("SetFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting formula: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions, object) {#setformula_1}

Imposta la formula e il valore (risultato calcolato) della formula.

```csharp
public void SetFormula(string formula, FormulaParseOptions options, object value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | La formula. |
| opzioni | FormulaParseOptions | Opzioni per l'analisi della formula. |
| valore | Object | Il valore (risultato calcolato) della formula. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Imposta la formula iniziale con riferimento al componente aggiuntivo
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Initial formula: " + sheet.Cells[0, 0].Formula);

            // Usa SetFormula per sovrascrivere senza controllare il componente aggiuntivo
            sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
            Console.WriteLine("After SetFormula: " + sheet.Cells[0, 0].Formula);

            // Ripristina alla formula del componente aggiuntivo
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Reset to add-in formula: " + sheet.Cells[0, 0].Formula);

            // Crea una nuova cartella di lavoro e copia il foglio
            Workbook wb2 = new Workbook();
            wb2.Worksheets[0].Cells[0, 0].Formula = "'externalDS.xlam'!dsfunnew(C1)";
            wb2.Worksheets[0].Copy(sheet);
            Console.WriteLine("After copy: " + wb2.Worksheets[0].Cells[0, 0].Formula);
        }
    }
}
```

### Vedi anche

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


