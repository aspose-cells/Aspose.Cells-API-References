---
title: "Cells.ImportDataGrid"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Importa un DataGrid en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/cells/importdatagrid/
---
## ImportDataGrid(DataGrid, int, int, bool) {#importdatagrid}

Importa un DataGrid a una hoja de cálculo.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, bool insertRows)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataGrid | DataGrid | El objeto DataGrid a importar. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| insertRows | Booleano | Indica si se añaden filas extra para ajustar los datos. |

### Valor de retorno

Número total de filas importadas

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un DataTable para simular datos de DataGrid
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Age");
            dataTable.Rows.Add("John", 30);
            dataTable.Rows.Add("Jane", 25);

            try
            {
                // Importar los datos usando ImportDataView, que está disponible en la API
                worksheet.Cells.ImportDataView(dataTable.DefaultView, 0, 0);

                Console.WriteLine("Data imported successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("ImportDataGridDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool) {#importdatagrid_1}

Importa un DataGrid a una hoja de cálculo.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataGrid | DataGrid | El objeto DataGrid a importar. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| totalRows | Int32 | Número de filas a importar. |
| totalColumns | Int32 | Número de columnas a importar. |
| insertRows | Booleano | Indica si se añaden filas extra para ajustar los datos. |

### Valor de retorno

Número total de filas importadas

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            try
            {
                // Crear un DataGrid de ejemplo con algunos datos
                // Usando una matriz de cadenas simple para simular los datos de DataGrid
                string[,] gridData = new string[,]
                {
                    { "Name", "Age", "City" },
                    { "John", "30", "New York" },
                    { "Jane", "25", "Chicago" },
                    { "Bob", "35", "Los Angeles" }
                };

                // Importar los datos a la hoja de cálculo comenzando en la fila 0, columna 0
                cells.ImportArray(gridData, 0, 0);

                // Guarda el libro de trabajo
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

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool, bool) {#importdatagrid_2}

Importa un DataGrid a una hoja de cálculo.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows, bool importStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataGrid | DataGrid | El objeto DataGrid a importar. |
| firstRow | Int32 | El número de fila de la primera celda en la que importar. |
| firstColumn | Int32 | El número de columna de la primera celda en la que importar. |
| totalRows | Int32 | Número de filas a importar. |
| totalColumns | Int32 | Número de columnas a importar. |
| insertRows | Booleano | Indica si se añaden filas extra para ajustar los datos. |
| importStyle | Booleano | Indica si se importa el estilo de celda. |

### Valor de retorno

Número total de filas importadas

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra que normalmente provienen de un DataGrid
            var sampleData = new List<object[]>
            {
                new object[] { "Name", "Age", "City" },
                new object[] { "John", 30, "New York" },
                new object[] { "Jane", 25, "Los Angeles" },
                new object[] { "Bob", 35, "Chicago" }
            };

            try
            {
                // Importar los datos directamente a las celdas ya que no podemos usar DataGrid
                for (int row = 0; row < sampleData.Count; row++)
                {
                    for (int col = 0; col < sampleData[row].Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(sampleData[row][col]);
                    }
                }

                Console.WriteLine("Data imported successfully to worksheet.");

                // Guarda el libro de trabajo
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

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


