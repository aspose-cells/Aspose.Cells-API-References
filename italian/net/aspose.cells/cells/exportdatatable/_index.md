---
title: "Cells.ExportDataTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Esporta i dati nella raccolta Cells in un oggetto DataTable"
type: docs
url: /it/net/aspose.cells/cells/exportdatatable/
---
## ExportDataTable(int, int, int, int) {#exportdatatable}

Esporta i dati nella raccolta [`Cells`](../) in un oggetto DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Il numero di riga della prima cella da esportare. |
| firstColumn | Int32 | Il numero di colonna della prima cella da esportare. |
| totalRows | Int32 | Numero di righe da importare. |
| totalColumns | Int32 | Numero di colonne da importare. |

### Valore di ritorno

Oggetto DataTable esportato.

### Osservazioni

Se utilizzi questo metodo per esportare un blocco di dati, assicurati che i dati in una colonna siano dello stesso tipo. In caso contrario, usa invece il metodo [`ExportDataTableAsString`](../exportdatatableasstring/).

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Person {i}");
                worksheet.Cells[i, 1].PutValue(20 + i);
                worksheet.Cells[i, 2].PutValue($"City {i}");
            }

            // Esporta i dati in DataTable (a partire dalla riga 0, colonna 0, con 5 righe e 3 colonne)
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 5, 3);

            // Visualizza i dati esportati
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(int, int, int, int, bool) {#exportdatatable_2}

Esporta i dati nella raccolta [`Cells`](../) in un oggetto DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool exportColumnName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Il numero di riga della prima cella da esportare. |
| firstColumn | Int32 | Il numero di colonna della prima cella da esportare. |
| totalRows | Int32 | Numero di righe da importare. |
| totalColumns | Int32 | Numero di colonne da importare. |
| exportColumnName | Booleano | Indica se i dati nella prima riga vengono esportati nel nome della colonna di DataTable. |

### Valore di ritorno

Oggetto DataTable esportato.

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Esporta i dati in DataTable (la prima riga contiene intestazioni)
            DataTable dt = worksheet.Cells.ExportDataTable(0, 0, 3, 2, true);

            // Visualizza i dati esportati
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTable(int, int, int, int, ExportTableOptions) {#exportdatatable_1}

Esporta i dati nella raccolta [`Cells`](../) in un oggetto DataTable.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    ExportTableOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Il numero di riga della prima cella da esportare. |
| firstColumn | Int32 | Il numero di colonna della prima cella da esportare. |
| totalRows | Int32 | Numero di righe da importare. |
| totalColumns | Int32 | Numero di colonne da importare. |
| opzioni | ExportTableOptions | Tutte le opzioni di esportazione della tabella |

### Valore di ritorno

Oggetto DataTable esportato.

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32ExportTablDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Imposta valore e formato per la cella A1
            cells["A1"].PutValue(1.23356);
            Style style = cells["A1"].GetStyle();
            style.Custom = "0.00";
            cells["A1"].SetStyle(style);

            // Crea opzioni di esportazione
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsString = true;

            // Esporta con la strategia di formato CellStyle
            etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
            DataTable dt1 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("CellStyle format: " + dt1.Rows[0][0].ToString());

            // Esporta con la strategia di formato None
            etOpt.FormatStrategy = CellValueFormatStrategy.None;
            DataTable dt2 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("None format: " + dt2.Rows[0][0].ToString());

            // Esporta con la strategia di formato DisplayStyle
            etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            DataTable dt3 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("DisplayStyle format: " + dt3.Rows[0][0].ToString());
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


