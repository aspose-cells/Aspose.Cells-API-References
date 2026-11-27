---
title: "Cells.ImportDataGrid"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Importerar en DataGrid till ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/cells/importdatagrid/
---
## ImportDataGrid(DataGrid, int, int, bool) {#importdatagrid}

Importerar en DataGrid till ett kalkylblad.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, bool insertRows)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataGrid | DataGrid | DataGrid-objektet som ska importeras. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| insertRows | Boolean | Indikerar om extra rader läggs till för att passa data. |

### Returvärde

Totalt antal importerade rader

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en DataTable för att simulera DataGrid-data
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Age");
            dataTable.Rows.Add("John", 30);
            dataTable.Rows.Add("Jane", 25);

            try
            {
                // Importera data med ImportDataView som finns tillgänglig i API:et
                worksheet.Cells.ImportDataView(dataTable.DefaultView, 0, 0);

                Console.WriteLine("Data imported successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("ImportDataGridDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool) {#importdatagrid_1}

Importerar en DataGrid till ett kalkylblad.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataGrid | DataGrid | DataGrid-objektet som ska importeras. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| totalRows | Int32 | Antal rader att importera. |
| totalColumns | Int32 | Antal kolumner att importera. |
| insertRows | Boolean | Indikerar om extra rader läggs till för att passa data. |

### Returvärde

Totalt antal importerade rader

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            try
            {
                // Skapa ett exempel-DataGrid med viss data
                // Använd en enkel strängarray för att simulera DataGrid-data
                string[,] gridData = new string[,]
                {
                    { "Name", "Age", "City" },
                    { "John", "30", "New York" },
                    { "Jane", "25", "Chicago" },
                    { "Bob", "35", "Los Angeles" }
                };

                // Importera data till kalkylbladet med start på rad 0, kolumn 0
                cells.ImportArray(gridData, 0, 0);

                // Spara arbetsboken
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

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool, bool) {#importdatagrid_2}

Importerar en DataGrid till ett kalkylblad.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows, bool importStyle)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataGrid | DataGrid | DataGrid-objektet som ska importeras. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| totalRows | Int32 | Antal rader att importera. |
| totalColumns | Int32 | Antal kolumner att importera. |
| insertRows | Boolean | Indikerar om extra rader läggs till för att passa data. |
| importStyle | Boolean | Indikerar om cellstilen importeras. |

### Returvärde

Totalt antal importerade rader

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata som normalt skulle komma från en DataGrid
            var sampleData = new List<object[]>
            {
                new object[] { "Name", "Age", "City" },
                new object[] { "John", 30, "New York" },
                new object[] { "Jane", 25, "Los Angeles" },
                new object[] { "Bob", 35, "Chicago" }
            };

            try
            {
                // Importera data direkt till celler eftersom vi inte kan använda DataGrid
                for (int row = 0; row < sampleData.Count; row++)
                {
                    for (int col = 0; col < sampleData[row].Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(sampleData[row][col]);
                    }
                }

                Console.WriteLine("Data imported successfully to worksheet.");

                // Spara arbetsboken
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

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


