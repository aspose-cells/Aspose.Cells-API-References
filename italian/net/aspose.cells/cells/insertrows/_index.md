---
title: "Cells.InsertRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Inserisce più righe nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/insertrows/
---
## InsertRows(int, int, bool) {#insertrows_2}

Inserisce più righe nel foglio di lavoro.

```csharp
public void InsertRows(int rowIndex, int totalRows, bool updateReference)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della riga. |
| totalRows | Int32 | Numero di righe da inserire. |
| updateReference | Booleano | Indica se i riferimenti in altri fogli di lavoro verranno aggiornati. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // Inserisci una riga all'indice 2 (diventerà la nuova riga 3)
            worksheet.Cells.InsertRows(2, 1, true);
            
            // Aggiungi dati alla riga inserita
            worksheet.Cells["A3"].PutValue("Inserted Data");
            
            // Salva la cartella di lavoro
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int, InsertOptions) {#insertrows_1}

Inserisce più righe nel foglio di lavoro.

```csharp
public void InsertRows(int rowIndex, int totalRows, InsertOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della riga. |
| totalRows | Int32 | Numero di righe da inserire. |
| opzioni | InsertOptions | Opzioni per l'operazione di inserimento. |

### Esempi

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcuni dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Inserisci 3 righe all'indice di riga 5 con le opzioni specificate
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            workbook.Save("InsertRowsWithOptions.xlsx");
        }
    }
}
```

### Vedi anche

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int) {#insertrows}

Inserisce più righe nel foglio di lavoro.

```csharp
public void InsertRows(int rowIndex, int totalRows)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | Int32 | Indice della riga. |
| totalRows | Int32 | Numero di righe da inserire. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi alcuni dati di esempio
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Data1");
            cells["B2"].PutValue("Data2");
            cells["A3"].PutValue("Data3");
            cells["B3"].PutValue("Data4");

            // Inserisci 2 righe all'indice di riga 2
            cells.InsertRows(2, 2);

            // Verifica che le righe inserite siano vuote
            Console.WriteLine("Cell A2 value: " + cells[1, 0].Value); // Should be "Data1"
            Console.WriteLine("Cell A3 value: " + cells[2, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A4 value: " + cells[3, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A5 value: " + cells[4, 0].Value); // Should be "Data3"

            // Salva la cartella di lavoro
            workbook.Save("InsertRowsDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


