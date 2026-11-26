---
title: "Cells.DeleteRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina varias filas"
type: docs
url: /es/net/aspose.cells/cells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Elimina varias filas.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | El índice de la primera fila a eliminar. |
| totalRows | Int32 | Cantidad de filas a eliminar. |

### Observaciones

Si el rango eliminado contiene la parte superior (no completa) de la tabla (ListObject), el rango no podrá ser eliminado y no se hará nada. Funciona de la misma manera que en MS Excel.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar algunos datos de muestra
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            Console.WriteLine("Before deleting rows:");
            PrintCellValues(cells, 0, 9, 0, 4);

            // Eliminar 2 filas a partir del índice de fila 2 (tercera fila)
            cells.DeleteRows(2, 2);

            Console.WriteLine("\nAfter deleting rows 3-4:");
            PrintCellValues(cells, 0, 7, 0, 4);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }

        private static void PrintCellValues(Cells cells, int startRow, int endRow, int startCol, int endCol)
        {
            for (int i = startRow; i <= endRow; i++)
            {
                for (int j = startCol; j <= endCol; j++)
                {
                    Console.Write($"{cells[i, j].StringValue}\t");
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

## DeleteRows(int, int, bool) {#deleterows_2}

Elimina varias filas en la hoja de cálculo.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de la primera fila a eliminar. |
| totalRows | Int32 | Cantidad de filas a eliminar. |
| updateReference | Booleano | Indica si se actualizan referencias en otras hojas de cálculo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Importar datos en celdas
            worksheet.Cells.ImportTwoDimensionArray(new object[2, 2] { { "A1", "B1" }, { "A2", "B2" } }, 0, 0);

            // Crear una tabla
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 1, 1, false)];
            table.ShowHeaderRow = false;

            Console.WriteLine("Before DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");

            // Eliminar fila en el índice 1 (segunda fila) con actualización de referencia
            worksheet.Cells.DeleteRows(1, 1, true);

            Console.WriteLine("\nAfter DeleteRows:");
            Console.WriteLine($"Table Data Range Row Count: {table.ListColumns.Count}");
            Console.WriteLine($"Table Start Row: {table.StartRow}");
            Console.WriteLine($"Table End Row: {table.EndRow}");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRows(int, int, DeleteOptions) {#deleterows_1}

Elimina varias filas en la hoja de cálculo.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, DeleteOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de la primera fila a eliminar. |
| totalRows | Int32 | Cantidad de filas a eliminar. |
| opciones | DeleteOptions | Opciones para la operación de eliminación |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Establecer datos de muestra y fórmulas
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].Formula = "=SUM(A1:A3)";
            
            // Eliminar fila 2 sin monitoreo (ya que FormulaChangeMonitor no está disponible)
            cells.DeleteRows(1, 1, new DeleteOptions());
            
            Console.WriteLine("Deleted row 2. Formula in B1 should now be: " + cells["B1"].Formula);
        }
    }
}
```

### Ver también

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


