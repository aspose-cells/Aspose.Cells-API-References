---
title: "Cells.Merge"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Unisce un intervallo specificato di celle in un'unica cella"
type: docs
url: /it/net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

Unisce un intervallo di celle specificato in un'unica cella.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Prima riga di questo intervallo (indice zero) |
| firstColumn | Int32 | Prima colonna di questo intervallo (indice zero) |
| totalRows | Int32 | Numero di righe (indice a base 1) |
| totalColumns | Int32 | Numero di colonne (indice a base 1) |

### Osservazioni

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra nell'intervallo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Inserisci valori nelle celle per dimostrare l'unione
            cells[0, 0].PutValue("Merged Area");
            cells[5, 5].PutValue("Not Merged");

            // Unisci le celle a partire dalla riga 0, colonna 0 estendendosi per 3 righe e 2 colonne
            cells.Merge(0, 0, 3, 2);

            // Salva la cartella di lavoro
            workbook.Save("MergeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

Unisce un intervallo di celle specificato in un'unica cella.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Prima riga di questo intervallo (indice zero) |
| firstColumn | Int32 | Prima colonna di questo intervallo (indice zero) |
| totalRows | Int32 | Numero di righe (indice a base 1) |
| totalColumns | Int32 | Numero di colonne (indice a base 1) |
| mergeConflict | Booleano | Intervalli uniti in conflitto di merge. |

### Osservazioni

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra nell'intervallo. Se mergeConflict è true e l'intervallo unito è in conflitto con altre celle unite, le altre celle unite verranno rimosse automaticamente.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Unisci le celle dalla riga 3, colonna 4 (D3) alla riga 7, colonna 5 (E7) - 5 righe e 2 colonne
            worksheet.Cells.Merge(3, 4, 5, 2, true);
            
            // Salva la cartella di lavoro
            workbook.Save("MergeDemoOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

Unisce un intervallo di celle specificato in un'unica cella.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Prima riga di questo intervallo (indice zero) |
| firstColumn | Int32 | Prima colonna di questo intervallo (indice zero) |
| totalRows | Int32 | Numero di righe (indice a base 1) |
| totalColumns | Int32 | Numero di colonne (indice a base 1) |
| checkConflict | Booleano | Indica se verificare se le celle unite si intersecano con altre celle unite |
| mergeConflict | Booleano | Intervalli uniti in conflitto di merge. |

### Osservazioni

Fai riferimento alla cella unita tramite l'indirizzo della cella in alto a sinistra nell'intervallo. Se mergeConflict è true e l'intervallo unito è in conflitto con altre celle unite, le altre celle unite verranno rimosse automaticamente.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanBooDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Inserisci alcuni dati nelle celle da unire
            cells[0, 1].PutValue("Merged Cell");
            cells[1, 1].PutValue("This will be merged");

            // Unisci le celle senza opzioni (unione semplice)
            cells.Merge(0, 1, 2, 2);
            Console.WriteLine("Cells merged without options");

            // Dividi prima per dimostrare la successiva unione
            cells.UnMerge(0, 1, 2, 2);

            // Unisci le celle con ignoreStyle=false e mergeConflict=true
            cells.Merge(0, 1, 2, 2, false, true);
            Console.WriteLine("Cells merged with ignoreStyle=false and mergeConflict=true");

            // Salva la cartella di lavoro
            workbook.Save("MergeCellsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


