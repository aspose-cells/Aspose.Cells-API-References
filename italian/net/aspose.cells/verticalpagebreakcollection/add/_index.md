---
title: "VerticalPageBreakCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VerticalPageBreakCollection. Aggiunge un'interruzione di pagina verticale alla raccolta"
type: docs
url: /it/net/aspose.cells/verticalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Aggiunge un'interruzione di pagina verticale alla collezione.

```csharp
public int Add(int startRow, int endRow, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | Int32 | Indice della riga iniziale, basato su zero. |
| endRow | Int32 | Indice della riga finale, basato su zero. |
| colonna | Int32 | Indice della colonna, a base zero. |

### Valore di ritorno

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Osservazioni

Questo metodo è usato per aggiungere un'interruzione di pagina verticale all'interno di un'area di stampa.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
            
            // Dimostrare Add con parametri (Int32, Int32, Int32)
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            
            // Esempi aggiuntivi per il contesto
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3

            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"{i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Aggiunge un'interruzione di pagina verticale alla collezione.

```csharp
public int Add(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | Indice della colonna della cella, a base zero. |

### Valore di ritorno

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Osservazioni

L'interruzione di pagina viene aggiunta nell'angolo in alto a sinistra della cella. Si prega di impostare contemporaneamente un'interruzione di pagina orizzontale e una verticale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Dimostrare il metodo Add con parametro Int32
            verticalPageBreaks.Add(4); // Add vertical page break at column 4

            // Stampa i dettagli dell'interruzione di pagina aggiunta
            VerticalPageBreak vpb = verticalPageBreaks[0];
            Console.WriteLine($"Vertical Page Break: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Aggiunge un'interruzione di pagina verticale alla collezione.

```csharp
public int Add(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga della cella, a base zero. |
| colonna | Int32 | Indice della colonna della cella, a base zero. |

### Valore di ritorno

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Osservazioni

L'interruzione di pagina viene aggiunta nell'angolo in alto a sinistra della cella. Si prega di impostare contemporaneamente un'interruzione di pagina orizzontale e una verticale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la raccolta delle interruzioni di pagina verticali
            VerticalPageBreakCollection vPageBreaks = worksheet.VerticalPageBreaks;

            // Aggiungi interruzioni di pagina verticali in diverse posizioni di colonna
            vPageBreaks.Add(0, 5);  // Add page break after column 5
            vPageBreaks.Add(0, 10); // Add page break after column 10
            vPageBreaks.Add(0, 15); // Add page break after column 15

            // Aggiungi alcuni dati di esempio per visualizzare le interruzioni di pagina
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
            }

            // Salva la cartella di lavoro
            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Aggiunge un'interruzione di pagina verticale alla collezione.

```csharp
public int Add(string cellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Nome della cella. |

### Valore di ritorno

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Osservazioni

L'interruzione di pagina viene aggiunta nell'angolo in alto a sinistra della cella. Si prega di impostare contemporaneamente un'interruzione di pagina orizzontale e una verticale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.VerticalPageBreaks.Add("G5");
            
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Vedi anche

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


