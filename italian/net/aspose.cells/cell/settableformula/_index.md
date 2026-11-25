---
title: "Cell.SetTableFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Crea una tabella di dati a due variabili per l'intervallo specificato a partire da questa cella"
type: docs
url: /it/net/aspose.cells/cell/settableformula/
---
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}

Crea una tabella dati a due variabili per l'intervallo specificato a partire da questa cella.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell, 
    string columnInputCell, object[][] values)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowNumber | Int32 | Numero di righe per popolare la formula. |
| columnNumber | Int32 | Numero di colonne per popolare la formula. |
| rowInputCell | String | la cella di input della riga |
| columnInputCell | String | la cella di input della colonna |
| valori | Object[][] | valori per le celle nell'intervallo della formula della tabella |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);

            // Cella di destinazione dove verrà impostata la formula della tabella
            Cell targetCell = worksheet.Cells["C3"];

            // Prepara i parametri per SetTableFormula
            int rowNumber = 3;
            int columnNumber = 2;
            string rowInputCell = "A1";
            string columnInputCell = "A2";
            object[][] values = new object[][]
            {
                new object[] { 1, 2 },    // Row 1 data
                new object[] { 3, 4 },    // Row 2 data
                new object[] { 5, 6 }     // Row 3 data
            };

            try
            {
                // Imposta la formula della tabella nella cella di destinazione
                targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);

                // Calcola le formule della cartella di lavoro per aggiornare i risultati
                workbook.CalculateFormula();

                Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}

Crea una tabella dati a una variabile per l'intervallo specificato a partire da questa cella.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput, 
    object[][] values)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowNumber | Int32 | Numero di righe per popolare la formula. |
| columnNumber | Int32 | Numero di colonne per popolare la formula. |
| inputCell | String | la cella di input |
| isRowInput | Booleano | Indica se la cella di input è una cella di input di riga (true) o una cella di input di colonna (false). |
| valori | Object[][] | valori per le celle nell'intervallo della formula della tabella |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(100000);
            cells[1, 3].PutValue(0.05);
            cells[1, 4].PutValue(2);
            cells[2, 1].PutValue(360);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);
            
            try
            {
                // Prepara i parametri per SetTableFormula
                int rowCount = 3;
                int colCount = 3;
                object[][] inputValues = new object[][] 
                {
                    new object[] { 0.05, 0.06, 0.07 },
                    new object[] { 1000, 2000, 3000 },
                    new object[] { 100, 200, 300 }
                };

                // Ottieni la cella di destinazione per la tabella dati (C3)
                Cell tableCell = worksheet.Cells["C3"];
                // Chiama SetTableFormula con variazioni del tasso di interesse
                tableCell.SetTableFormula(
                    rowNumber: rowCount,
                    columnNumber: colCount,
                    inputCell: "A1",
                    isRowInput: true,
                    values: inputValues
                );

                // Calcola le formule per aggiornare i risultati della tabella
                workbook.CalculateFormula();

                Console.WriteLine("Data table created successfully with varying interest rates");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating data table: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}

Crea una tabella dati a due variabili per l'intervallo specificato a partire da questa cella.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, 
    int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, 
    object[][] values)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowNumber | Int32 | Numero di righe per popolare la formula. |
| columnNumber | Int32 | Numero di colonne per popolare la formula. |
| rowIndexOfRowInputCell | Int32 | indice di riga della cella di input della riga |
| columnIndexOfRowInputCell | Int32 | indice di colonna della cella di input della riga |
| rowIndexOfColumnInputCell | Int32 | indice di riga della cella di input della colonna |
| columnIndexOfColumnInputCell | Int32 | indice di colonna della cella di input della colonna |
| valori | Object[][] | valori per le celle nell'intervallo della formula della tabella |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[1, 4].PutValue(4);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);
            
            Cell formulaCell = cells[2, 2];

            // Prepara i valori di input per la tabella dati (tassi di interesse e importi del prestito)
            object[][] tableValues = new object[3][];
            tableValues[0] = new object[] { 0.05, 0.06, 0.07 };
            tableValues[1] = new object[] { 1000, 2000, 3000 };
            tableValues[2] = new object[] { 100, 200, 300 };

            try
            {
                // Imposta la formula della tabella con dimensioni della tabella dati 3x3 e offset della cella di input
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 3,
                    rowIndexOfRowInputCell: 0,  
                    columnIndexOfRowInputCell: 0,   
                    rowIndexOfColumnInputCell: 1,   
                    columnIndexOfColumnInputCell: 0, 
                    values: tableValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Data table formula set successfully. Check B2:D4 in output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            workbook.Save("CellTableFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}

Crea una tabella dati a una variabile per l'intervallo specificato a partire da questa cella.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, 
    int columnIndexOfInputCell, bool isRowInput, object[][] values)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowNumber | Int32 | Numero di righe per popolare la formula. |
| columnNumber | Int32 | Numero di colonne per popolare la formula. |
| rowIndexOfInputCell | Int32 | indice di riga della cella di input |
| columnIndexOfInputCell | Int32 | indice di colonna della cella di input |
| isRowInput | Booleano | Indica se la cella di input è una cella di input di riga (true) o una cella di input di colonna (false). |
| valori | Object[][] | valori per le celle nell'intervallo della formula della tabella |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(20);
            cells[1, 3].PutValue(30);            
            cells[2, 1].PutValue(20);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);

            // Crea un array di dati di esempio per i parametri della formula della tabella
            object[][] inputValues = new object[][]
            {
                new object[] { 10, 20 },
                new object[] { 30, 40 },
                new object[] { 50, 60 }
            };

            // Ottieni la cella target per applicare la formula della tabella
            Cell formulaCell = worksheet.Cells[2, 2];

            try
            {
                // Imposta la formula della tabella con: 
                // 3 righe, 2 colonne, cella di input in A1 (0,0), 
                // tipo di input della riga, e valori di esempio
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 2,
                    rowIndexOfInputCell: 0,
                    columnIndexOfInputCell: 0,
                    isRowInput: true,
                    values: inputValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Table formula applied successfully. " + 
                    "Saved workbook with 3x2 table formula at C3.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("TableFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


