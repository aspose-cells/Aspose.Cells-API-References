---
title: "Cells.ImportDataGrid"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Importa un DataGrid in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/cells/importdatagrid/
---
## ImportDataGrid(DataGrid, int, int, bool) {#importdatagrid}

Importa un DataGrid in un foglio di lavoro.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, bool insertRows)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataGrid | DataGrid | L'oggetto DataGrid da importare. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| insertRows | Booleano | Indica se vengono aggiunte righe extra per adattare i dati. |

### Valore di ritorno

Numero totale di righe importate

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;
    using System.Data;

    public class CellsMethodImportDataGridWithDataGridInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un DataTable per simulare i dati del DataGrid
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Age");
            dataTable.Rows.Add("John", 30);
            dataTable.Rows.Add("Jane", 25);

            try
            {
                // Importa i dati usando ImportDataView, disponibile nell'API
                worksheet.Cells.ImportDataView(dataTable.DefaultView, 0, 0);

                Console.WriteLine("Data imported successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("ImportDataGridDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool) {#importdatagrid_1}

Importa un DataGrid in un foglio di lavoro.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataGrid | DataGrid | L'oggetto DataGrid da importare. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| totalRows | Int32 | Numero di righe da importare. |
| totalColumns | Int32 | Numero di colonne da importare. |
| insertRows | Booleano | Indica se vengono aggiunte righe extra per adattare i dati. |

### Valore di ritorno

Numero totale di righe importate

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            try
            {
                // Crea un DataGrid di esempio con alcuni dati
                // Utilizzare un semplice array di stringhe per simulare i dati del DataGrid
                string[,] gridData = new string[,]
                {
                    { "Name", "Age", "City" },
                    { "John", "30", "New York" },
                    { "Jane", "25", "Chicago" },
                    { "Bob", "35", "Los Angeles" }
                };

                // Importa i dati nel foglio di lavoro a partire dalla riga 0, colonna 0
                cells.ImportArray(gridData, 0, 0);

                // Salva la cartella di lavoro
                workbook.Save("ImportDataGridDemo.xlsx");
                Console.WriteLine("Data imported successfully to ImportDataGridDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
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

## ImportDataGrid(DataGrid, int, int, int, int, bool, bool) {#importdatagrid_2}

Importa un DataGrid in un foglio di lavoro.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows, bool importStyle)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dataGrid | DataGrid | L'oggetto DataGrid da importare. |
| firstRow | Int32 | Il numero di riga della prima cella in cui importare. |
| firstColumn | Int32 | Il numero di colonna della prima cella in cui importare. |
| totalRows | Int32 | Numero di righe da importare. |
| totalColumns | Int32 | Numero di colonne da importare. |
| insertRows | Booleano | Indica se vengono aggiunte righe extra per adattare i dati. |
| importStyle | Booleano | Indica se importare lo stile della cella. |

### Valore di ritorno

Numero totale di righe importate

### Esempi

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32Bo257661Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio che normalmente provengono da un DataGrid
            var sampleData = new List<object[]>
            {
                new object[] { "Name", "Age", "City" },
                new object[] { "John", 30, "New York" },
                new object[] { "Jane", 25, "Los Angeles" },
                new object[] { "Bob", 35, "Chicago" }
            };

            try
            {
                // Importa i dati direttamente nelle celle poiché non possiamo usare il DataGrid
                for (int row = 0; row < sampleData.Count; row++)
                {
                    for (int col = 0; col < sampleData[row].Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(sampleData[row][col]);
                    }
                }

                Console.WriteLine("Data imported successfully to worksheet.");

                // Salva la cartella di lavoro
                workbook.Save("ImportDataGridDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


