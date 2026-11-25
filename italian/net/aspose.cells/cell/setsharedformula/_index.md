---
title: "Cell.SetSharedFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Imposta una formula per un intervallo di celle"
type: docs
url: /it/net/aspose.cells/cell/setsharedformula/
---
## SetSharedFormula(string, int, int, bool, bool) {#setsharedformula_3}

Imposta una formula per un intervallo di celle.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sharedFormula | String | Formula condivisa. |
| rowNumber | Int32 | Numero di righe per popolare la formula. |
| columnNumber | Int32 | Numero di colonne per popolare la formula. |
| isR1C1 | Booleano | se la formula è una formula R1C1 |
| isLocal | Booleano | se la formula è formattata per locale |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2019. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            // Popola dati di esempio nella colonna A
            for (int row = 0; row < 5; row++)
            {
                cells[row, 0].Value = row + 1; // A1-A5: 1-5
            }

            // Ottieni la cella target B1 per impostare la formula condivisa
            Cell targetCell = cells[0, 1]; // B1

            try
            {
                // Imposta la formula condivisa per calcolare il quadrato dei valori nella colonna A
                // Parametri: (formula, rowCount=5, columnCount=1, isR1C1=false, isLocal=false)
#pragma warning disable 0618 // Disable obsolete warning for demonstration
                targetCell.SetSharedFormula("=A1^2", 5, 1, false, false);
#pragma warning restore 0618

                // Verifica la propagazione della formula
                Console.WriteLine($"B1 formula: {targetCell.Formula}");
                Console.WriteLine($"B5 formula: {cells[4, 1].Formula}");

                // Calcola la cartella di lavoro per aggiornare i risultati della formula
                workbook.CalculateFormula();

                Console.WriteLine($"A1 value: {cells["A1"].Value}");
                Console.WriteLine($"A5 value: {cells["A5"].Value}");
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B5 value: {cells[4, 1].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
                return;
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("SetSharedFormulaDemo.xlsx");
            Console.WriteLine("Spreadsheet saved successfully.");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int) {#setsharedformula}

Imposta formule condivise a un intervallo di celle.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sharedFormula | String | Formula condivisa. |
| rowNumber | Int32 | Numero di righe per popolare la formula. |
| columnNumber | Int32 | Numero di colonne per popolare la formula. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetSharedFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta una formula condivisa nella colonna B a partire da B1 fino a B20
            cells["B1"].SetSharedFormula("=C1*2", 20, 1);

            // Imposta alcuni valori nella colonna C per dimostrare il calcolo della formula
            for (int i = 0; i < 20; i++)
            {
                cells[i, 2].PutValue(i + 1); // Column C values (C1=1, C2=2...)
            }

            // Calcola le formule
            workbook.CalculateFormula();

            // Genera i risultati per la verifica
            for (int i = 0; i < 5; i++) // Display first 5 results
            {
                Console.WriteLine($"B{i+1} value: {cells[i, 1].Value}");
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

## SetSharedFormula(string, int, int, FormulaParseOptions) {#setsharedformula_1}

Imposta formule condivise a un intervallo di celle.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sharedFormula | String | Formula condivisa. |
| rowNumber | Int32 | Numero di righe per popolare la formula. |
| columnNumber | Int32 | Numero di colonne per popolare la formula. |
| opzioni | FormulaParseOptions | Opzioni per l'analisi della formula. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio nella colonna A
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Ottieni la cella target dove imposteremo la formula condivisa
            Cell targetCell = worksheet.Cells["B1"];

            try
            {
                // Crea opzioni di analisi della formula con impostazioni predefinite
                FormulaParseOptions options = new FormulaParseOptions();

                // Imposta la formula condivisa per 3 righe e 2 colonne a partire da B1
                targetCell.SetSharedFormula("=A1*2", 3, 2, options);

                Console.WriteLine("Shared formula set successfully for B1:C3 range");
                Console.WriteLine("B1 formula: " + worksheet.Cells["B1"].Formula);
                Console.WriteLine("C3 formula: " + worksheet.Cells["C3"].Formula);

                workbook.CalculateFormula();
                Console.WriteLine("B3 value: " + worksheet.Cells["B3"].Value);
                Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
                Console.WriteLine("C3 value: " + worksheet.Cells["C3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("SetSharedFormulaDemo.xlsx");
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

## SetSharedFormula(string, int, int, FormulaParseOptions, object[][]) {#setsharedformula_2}

Imposta formule condivise a un intervallo di celle.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sharedFormula | String | Formula condivisa. |
| rowNumber | Int32 | Numero di righe per popolare la formula. |
| columnNumber | Int32 | Numero di colonne per popolare la formula. |
| opzioni | FormulaParseOptions | Opzioni per l'analisi della formula. |
| valori | Object[][] | valori per quelle celle con la formula condivisa data |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo1
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta valore di esempio nella cella A1
            worksheet.Cells["A1"].PutValue(5);

            // Ottieni la cella di destinazione B2 dove verrà impostata la formula condivisa
            Cell cell = worksheet.Cells["B2"];

            try
            {
                // Definisci i parametri della formula condivisa
                string formula = "=A1*2";
                int totalRows = 2;
                int totalColumns = 2;
                FormulaParseOptions parseOptions = new FormulaParseOptions();
                object[][] presetValues = new object[2][]
                {
                    new object[] { 10, 10 },
                    new object[] { 10, 10 }
                };

                // Imposta la formula condivisa per un intervallo 2x2 che inizia da B2 con valori predefiniti
                cell.SetSharedFormula(formula, totalRows, totalColumns, parseOptions, presetValues);

                Console.WriteLine("Shared formula set successfully. Cells B2:C3 contain values 10");
                workbook.CalculateFormula();
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "C3");
                IEnumerator iter = range.GetEnumerator();
                while(iter.MoveNext()) 
                {
                    Cell temp = (Cell)iter.Current;
                    Console.WriteLine(temp.Name + "  " + temp.Value);
                }

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("SetSharedFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


