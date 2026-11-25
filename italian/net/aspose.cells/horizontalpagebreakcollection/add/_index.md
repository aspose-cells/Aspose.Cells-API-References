---
title: "HorizontalPageBreakCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo HorizontalPageBreakCollection. Aggiunge un'interruzione di pagina orizzontale alla collezione"
type: docs
url: /it/net/aspose.cells/horizontalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Aggiunge un'interruzione di pagina orizzontale alla raccolta.

```csharp
public int Add(int row, int startColumn, int endColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice di riga, basato su zero. |
| startColumn | Int32 | Indice di colonna iniziale, basato su zero. |
| endColumn | Int32 | Indice di colonna finale, basato su zero. |

### Valore di ritorno

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Osservazioni

Questo metodo è usato per aggiungere un'interruzione di pagina orizzontale all'interno di un'area di stampa.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dimostra il metodo Add con parametri (Int32, Int32, Int32)
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Aggiunge un'interruzione di pagina orizzontale alla raccolta.

```csharp
public int Add(int row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga della cella, a base zero. |

### Valore di ritorno

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Osservazioni

L'interruzione di pagina viene aggiunta nell'angolo in alto a sinistra della cella. Si prega di impostare contemporaneamente un'interruzione di pagina orizzontale e una verticale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi interruzioni di pagina orizzontali usando il parametro Int32
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Aggiunge un'interruzione di pagina orizzontale alla raccolta.

```csharp
public int Add(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga della cella, a base zero. |
| colonna | Int32 | Indice della colonna della cella, a base zero. |

### Valore di ritorno

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Osservazioni

L'interruzione di pagina viene aggiunta nell'angolo in alto a sinistra della cella. Si prega di impostare contemporaneamente un'interruzione di pagina orizzontale e una verticale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio per creare più righe
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Aggiungi interruzioni di pagina orizzontali a righe specifiche
            worksheet.HorizontalPageBreaks.Add(9, 0);  // Page break after row 9
            worksheet.HorizontalPageBreaks.Add(19, 0); // Page break after row 19
            worksheet.HorizontalPageBreaks.Add(29, 0); // Page break after row 29

            // Salva la cartella di lavoro
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Aggiunge un'interruzione di pagina orizzontale alla raccolta.

```csharp
public int Add(string cellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Nome della cella. |

### Valore di ritorno

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Osservazioni

L'interruzione di pagina viene aggiunta nell'angolo in alto a sinistra della cella. Si prega di impostare contemporaneamente un'interruzione di pagina orizzontale e una verticale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'interruzione di pagina orizzontale alla riga 4 (D5 è la riga 4 nell'indice basato su zero)
            worksheet.HorizontalPageBreaks.Add("D5");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


