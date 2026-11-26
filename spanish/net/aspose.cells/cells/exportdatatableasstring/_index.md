---
title: "Cells.ExportDataTableAsString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Exporta datos de la colección Cells a un objeto DataTable"
type: docs
url: /es/net/aspose.cells/cells/exportdatatableasstring/
---
## ExportDataTableAsString(int, int, int, int) {#exportdatatableasstring}

Exporta datos de la colección [`Cells`](../) a un objeto DataTable.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | El número de fila de la primera celda a exportar. |
| firstColumn | Int32 | El número de columna de la primera celda a exportar. |
| totalRows | Int32 | Número de filas a importar. |
| totalColumns | Int32 | Número de columnas a importar. |

### Valor de retorno

Objeto DataTable exportado.

### Observaciones

Todos los datos en la colección [`Cells`](../) se convierten a cadenas.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de muestra a las celdas
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");

            // Exportar datos a DataTable como cadenas
            DataTable dataTable = cells.ExportDataTableAsString(0, 0, 2, 2);

            // Mostrar los datos exportados
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

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ExportDataTableAsString(int, int, int, int, bool) {#exportdatatableasstring_1}

Exporta datos de la colección [`Cells`](../) a un objeto DataTable.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool exportColumnName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | El número de fila de la primera celda a exportar. |
| firstColumn | Int32 | El número de columna de la primera celda a exportar. |
| totalRows | Int32 | Número de filas a importar. |
| totalColumns | Int32 | Número de columnas a importar. |
| exportColumnName | Booleano | Indica si los datos de la primera fila se exportan al nombre de columna del DataTable. |

### Valor de retorno

Objeto DataTable exportado.

### Observaciones

Todos los datos en la colección [`Cells`](../) se convierten a cadenas.

### Ejemplos

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
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Exportar datos a DataTable
            int maxRow = worksheet.Cells.MaxDataRow + 1;
            int maxCol = worksheet.Cells.MaxDataColumn + 1;
            DataTable dataTable = worksheet.Cells.ExportDataTableAsString(0, 0, maxRow, maxCol, true);

            // Mostrar los datos exportados
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

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


