---
title: "Cells.ImportArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells."
type: docs
url: /it/net/aspose.cells/cells/importarray/
---
## ImportArray(string[], int, int) {#importarray_4}

```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn)
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(string[], int, int, bool) {#importarray_5}

Importa un array di string in un foglio di lavoro.

```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringArray | String[] | Array di stringhe. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| isVertical | Booleano | Specifica se importare i dati verticalmente o orizzontalmente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithStringInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati dell'array di stringhe
            string[] fruitArray = new string[] { "Apple", "Banana", "Cherry", "Date", "Elderberry" };

            try
            {
                // Chiama ImportArray con i parametri: (String[], Int32, Int32, Boolean)
                // Inizia l'importazione dalla riga 2 (3ª riga), colonna 1 (colonna B), verticalmente
                worksheet.Cells.ImportArray(fruitArray, 2, 1, true);

                Console.WriteLine("Imported string array vertically starting from cell B3:");
                foreach (string fruit in fruitArray)
                {
                    Console.WriteLine(fruit);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("CellsMethodImportArrayWithStringInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(int[], int, int) {#importarray_2}

```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn)
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(int[], int, int, bool) {#importarray_3}

Importa un array di integer in un foglio di lavoro.

```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intArray | Int32[] | Array di interi. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| isVertical | Booleano | Specifica se importare i dati verticalmente o orizzontalmente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithInt32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara i dati dell'array Int32
            int[] data = new int[] { 1, 2, 3, 4, 5 };

            try
            {
                // Chiama ImportArray con i parametri: (Int32[], firstRow=2, firstColumn=1, isVertical=true)
                worksheet.Cells.ImportArray(data, 2, 1, true);

                Console.WriteLine("Imported array vertically starting from cell B3:");
                for (int i = 0; i < data.Length; i++)
                {
                    Console.WriteLine($"Cell B{3 + i}: {worksheet.Cells[2 + i, 1].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("CellsMethodImportArrayWithInt32Int32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(double[], int, int) {#importarray}

```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn)
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(double[], int, int, bool) {#importarray_1}

Importa un array di double in un foglio di lavoro.

```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| doubleArray | Double[] | Array di double. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| isVertical | Booleano | Specifica se importare i dati verticalmente o orizzontalmente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithDoubleInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Prepara dati di esempio per l'array double
            double[] dataArray = new double[] { 1.23, 4.56, 7.89, 10.11, 12.13 };
            const int targetRow = 2;    // 0-based row index (3rd row)
            const int targetColumn = 1; // 0-based column index (2nd column)
            const bool isVertical = true;

            try
            {
                // Ottieni la collezione di celle e chiama ImportArray
                Cells cells = worksheet.Cells;
                cells.ImportArray(dataArray, targetRow, targetColumn, isVertical);
                
                Console.WriteLine($"Imported {dataArray.Length} double values starting at row {targetRow + 1}, column {targetColumn + 1}");
                Console.WriteLine($"Data orientation: {(isVertical ? "Vertical" : "Horizontal")}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("CellsImportArrayDoubleVerticalDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


