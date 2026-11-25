---
title: "Cells.InsertColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Inserisce alcune colonne nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/insertcolumns/
---
## InsertColumns(int, int) {#insertcolumns}

Inserisce alcune colonne nel foglio di lavoro.

```csharp
public void InsertColumns(int columnIndex, int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice colonna. |
| totalColumns | Int32 | Il numero di colonne. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inserisci 3 colonne a partire dall'indice colonna 1 (seconda colonna)
            worksheet.Cells.InsertColumns(1, 3);
            
            // Aggiungi dati di esempio per dimostrare le colonne inserite
            worksheet.Cells["A1"].PutValue("Original Column");
            worksheet.Cells["B1"].PutValue("Inserted Column 1");
            worksheet.Cells["C1"].PutValue("Inserted Column 2");
            worksheet.Cells["D1"].PutValue("Inserted Column 3");
            worksheet.Cells["E1"].PutValue("Original Column 2");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, bool) {#insertcolumns_2}

Inserisce alcune colonne nel foglio di lavoro.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice colonna. |
| totalColumns | Int32 | Il numero di colonne. |
| updateReference | Booleano | Indica se i riferimenti in altri fogli di lavoro verranno aggiornati. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inserisci 3 colonne all'indice colonna 2 (basato su zero), spostando le colonne esistenti a destra
            worksheet.Cells.InsertColumns(2, 3, true);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, InsertOptions) {#insertcolumns_1}

Inserisce alcune colonne nel foglio di lavoro.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, InsertOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | Indice colonna. |
| totalColumns | Int32 | Il numero di colonne. |
| opzioni | InsertOptions | Le opzioni per l'operazione di inserimento. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // Crea opzioni di inserimento
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.Clear;

            // Inserisci una colonna all'indice 1 (seconda colonna)
            worksheet.Cells.InsertColumns(1, 1, options);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


