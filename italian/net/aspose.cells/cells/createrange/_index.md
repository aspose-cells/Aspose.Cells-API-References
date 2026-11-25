---
title: "Cells.CreateRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Crea un oggetto Range da un intervallo di celle"
type: docs
url: /it/net/aspose.cells/cells/createrange/
---
## CreateRange(string, string) {#createrange_3}

Crea un oggetto [`Range`](../../range/) da un intervallo di celle.

```csharp
public Range CreateRange(string upperLeftCell, string lowerRightCell)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| upperLeftCell | String | Nome della cella in alto a sinistra. |
| lowerRightCell | String | Nome della cella in basso a destra. |

### Valore di ritorno

Un oggetto [`Range`](../../range/)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Crea un intervallo da A1 a A2
            Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
            range.Name = "MyRange";
            
            // Imposta i valori nell'intervallo
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            
            // Usa l'intervallo in una formula
            cells["B1"].Formula = "=SUM(MyRange)";
            
            // Calcola la formula
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of MyRange (A1:A2) is: " + cells["B1"].IntValue);
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, int, int) {#createrange_1}

Crea un oggetto [`Range`](../../range/) da un intervallo di celle.

```csharp
public Range CreateRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Prima riga di questo intervallo |
| firstColumn | Int32 | Prima colonna di questo intervallo |
| totalRows | Int32 | Numero di righe |
| totalColumns | Int32 | Numero di colonne |

### Valore di ritorno

Un oggetto [`Range`](../../range/)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea l'intervallo di origine (riga iniziale 2, colonna 2 con 3 righe e 4 colonne)
            Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);

            // Riempire l'intervallo di origine con dati di esempio
            for (int i = 0; i < rangeSrc.RowCount; i++)
            {
                for (int j = 0; j < rangeSrc.ColumnCount; j++)
                {
                    rangeSrc[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Crea l'intervallo di destinazione (riga iniziale 8, colonna 0 con le stesse dimensioni)
            Aspose.Cells.Range rangeDest = cells.CreateRange(8, 0, 3, 4);

            // Copia i valori dalla sorgente alla destinazione
            rangeDest.CopyValue(rangeSrc);

            // Salva la cartella di lavoro
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(string) {#createrange_2}

Crea un oggetto [`Range`](../../range/) da un indirizzo dell'intervallo.

```csharp
public Range CreateRange(string address)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| address | String | L'indirizzo dell'intervallo. |

### Valore di ritorno

Un oggetto [`Range`](../../range/)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un intervallo usando l'indirizzo stringa
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Riempire i dati nell'intervallo
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Crea un altro intervallo in un nuovo foglio di lavoro
            workbook.Worksheets.Add();
            Worksheet worksheet2 = workbook.Worksheets[1];
            Aspose.Cells.Range range2 = worksheet2.Cells.CreateRange("A1:C3");

            // Copia i dati tra gli intervalli
            range2.Copy(range);

            // Salva la cartella di lavoro
            workbook.Save("CreateRangeWithStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, bool) {#createrange}

Crea un oggetto [`Range`](../../range/) da righe di celle o colonne di celle.

```csharp
public Range CreateRange(int firstIndex, int number, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | Int32 | Indice della prima riga o indice della prima colonna, basato su zero. |
| numero | Int32 | Numero totale di righe o colonne, basato su uno. |
| isVertical | Booleano | True - Intervallo creato da colonne di celle. False - Intervallo creato da righe di celle. |

### Valore di ritorno

Un oggetto [`Range`](../../range/).

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea un intervallo a partire dalla cella A1 (0,0) con 5 righe e 3 colonne
            Aspose.Cells.Range range = cells.CreateRange(0, 0, true);

            // Riempire alcuni dati nell'intervallo
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Row {i}, Col {j}");
                }
            }

            // Salva la cartella di lavoro
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


