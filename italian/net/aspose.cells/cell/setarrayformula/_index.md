---
title: "Cell.SetArrayFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Imposta una formula di matrice a un intervallo di celle"
type: docs
url: /it/net/aspose.cells/cell/setarrayformula/
---
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}

Imposta una formula di matrice a un intervallo di celle.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | String | Formula di matrice. |
| rowNumber | Int32 | Numero di righe per popolare il risultato della formula di matrice. |
| columnNumber | Int32 | Numero di colonne per popolare il risultato della formula di matrice. |
| isR1C1 | Booleano | se la formula è una formula R1C1 |
| isLocal | Booleano | se la formula è formattata per locale |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Questa proprietà sarà rimossa 12 mesi dopo da dicembre 2019. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetArrayFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;

            try
            {
                // Ottieni la cella di destinazione dove vogliamo impostare la formula di matrice
                Cell targetCell = worksheet.Cells["B1"];

                // Imposta una formula di matrice che moltiplica i valori in A1:A3 per 2
                // Parametri: (formula, rowNumber=3, columnNumber=1, isR1C1=false, isLocal=false)
                targetCell.SetArrayFormula("=A1:A3*2", 3, 1, false, false);

                // Calcola la cartella di lavoro per vedere i risultati
                workbook.CalculateFormula();

                // Visualizza i risultati
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B2 value: {worksheet.Cells["B2"].Value}");
                Console.WriteLine($"B3 value: {worksheet.Cells["B3"].Value}");

                // Salva la cartella di lavoro
                workbook.Save("SetArrayFormulaDemo.xlsx");
                Console.WriteLine("Array formula set successfully and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting array formula: {ex.Message}");
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

## SetArrayFormula(string, int, int) {#setarrayformula}

Imposta una formula di matrice (formula di matrice legacy inserita tramite CTRL+SHIFT+ENTER in MS Excel) a un intervallo di celle.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | String | Formula di matrice. |
| rowNumber | Int32 | Numero di righe per popolare il risultato della formula di matrice. |
| columnNumber | Int32 | Numero di colonne per popolare il risultato della formula di matrice. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            Cell cell = cells["A1"];
            cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);

            workbook.CalculateFormula();

            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1} value: {cells[i, 0].IntValue}");
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

## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}

Imposta una formula di matrice a un intervallo di celle.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | String | Formula di matrice. |
| rowNumber | Int32 | Numero di righe per popolare il risultato della formula di matrice. |
| columnNumber | Int32 | Numero di colonne per popolare il risultato della formula di matrice. |
| opzioni | FormulaParseOptions | Opzioni per l'analisi della formula. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Inserisci dati di esempio nelle celle C1:E1
            cells["C1"].PutValue(10);
            cells["D1"].PutValue(20);
            cells["E1"].PutValue(30);

            // Imposta la formula di matrice nella cella A1 che si espanderà a 2 righe e 3 colonne
            cells["A1"].SetArrayFormula("=TRANSPOSE(C1:E1)", 2, 1, new FormulaParseOptions());

            // Calcola le formule
            workbook.CalculateFormula();

            // Restituisci i risultati
            Console.WriteLine("Array formula results:");
            for (int row = 0; row < 2; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = cells[row, col];
                    Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                }
            }
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

## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}

Imposta una formula di matrice a un intervallo di celle.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arrayFormula | String | Formula di matrice. |
| rowNumber | Int32 | Numero di righe per popolare il risultato della formula di matrice. |
| columnNumber | Int32 | Numero di colonne per popolare il risultato della formula di matrice. |
| opzioni | FormulaParseOptions | Opzioni per l'analisi della formula. |
| valori | Object[][] | valori per quelle celle con la formula di matrice data |

### Vedi anche

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


