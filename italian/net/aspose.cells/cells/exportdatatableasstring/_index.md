---
title: "Cells.ExportDataTableAsString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Esporta i dati nella raccolta Cells in un oggetto DataTable"
type: docs
url: /it/net/aspose.cells/cells/exportdatatableasstring/
---
## ExportDataTableAsString(int, int, int, int) {#exportdatatableasstring}

Esporta i dati nella raccolta [`Cells`](../) in un oggetto DataTable.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
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

Tutti i dati nella collezione [`Cells`](../) sono convertiti in stringhe.

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio alle celle
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");

            // Esporta i dati in DataTable come stringhe
            DataTable dataTable = cells.ExportDataTableAsString(0, 0, 2, 2);

            // Visualizza i dati esportati
            Console.WriteLine("Exported DataTable:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.Write(column.ColumnName + "\t");
            }
            Console.WriteLine();
            
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item.ToString() + "\t");
                }
                Console.WriteLine();
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

## ExportDataTableAsString(int, int, int, int, bool) {#exportdatatableasstring_1}

Esporta i dati nella raccolta [`Cells`](../) in un oggetto DataTable.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool exportColumnName)
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

### Osservazioni

Tutti i dati nella collezione [`Cells`](../) sono convertiti in stringhe.

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32BooleanDemo
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

            // Esporta i dati in DataTable
            int maxRow = worksheet.Cells.MaxDataRow + 1;
            int maxCol = worksheet.Cells.MaxDataColumn + 1;
            DataTable dataTable = worksheet.Cells.ExportDataTableAsString(0, 0, maxRow, maxCol, true);

            // Visualizza i dati esportati
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (DataColumn col in dataTable.Columns)
                {
                    Console.Write(row[col] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


