---
title: "Cells.RemoveDuplicates"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina filas duplicadas en la hoja"
type: docs
url: /es/net/aspose.cells/cells/removeduplicates/
---
## RemoveDuplicates() {#removeduplicates}

Elimina filas duplicadas en la hoja.

```csharp
public void RemoveDuplicates()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveDuplicatesDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Rellena celdas con algunos valores duplicados
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    // Crea duplicados en cada segunda fila
                    cells[i, j].PutValue(i % 2 == 0 ? "Duplicate" : $"Unique_{i}_{j}");
                }
            }

            Console.WriteLine($"Before RemoveDuplicates: {cells.Count} cells");
            
            // Eliminar valores duplicados
            cells.RemoveDuplicates();

            Console.WriteLine($"After RemoveDuplicates: {cells.Count} cells");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int) {#removeduplicates_1}

Elimina valores duplicados en el rango.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | La fila de inicio. |
| startColumn | Int32 | La columna de inicio |
| endRow | Int32 | El índice de fila final. |
| endColumn | Int32 | El índice de columna final. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo con duplicados
            cells["A1"].PutValue("Apple");
            cells["A2"].PutValue("Orange");
            cells["A3"].PutValue("Apple");
            cells["A4"].PutValue("Banana");
            cells["A5"].PutValue("Orange");

            // Eliminar duplicados de la columna A (índice basado en 0)
            cells.RemoveDuplicates(0, 0, 5, 0);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int, bool, int[]) {#removeduplicates_2}

Elimina datos duplicados del rango.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn, 
    bool hasHeaders, int[] columnOffsets)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | La fila de inicio. |
| startColumn | Int32 | La columna de inicio |
| endRow | Int32 | El índice de fila final. |
| endColumn | Int32 | El índice de columna final. |
| hasHeaders | Booleano | Indica si el rango contiene encabezados. |
| columnOffsets | Int32[] | Los desplazamientos de columna. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodRemoveDuplicatesWithInt32Int32Int32Int32BooleanIntDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Rellenar datos de ejemplo con duplicados
            cells[0, 0].PutValue("ID");
            cells[0, 1].PutValue("Name");
            cells[0, 2].PutValue("Age");
            
            cells[1, 0].PutValue(1);
            cells[1, 1].PutValue("John");
            cells[1, 2].PutValue(30);

            cells[2, 0].PutValue(2);
            cells[2, 1].PutValue("Jane");
            cells[2, 2].PutValue(25);

            cells[3, 0].PutValue(1); // Duplicate ID
            cells[3, 1].PutValue("John"); // Duplicate Name
            cells[3, 2].PutValue(35);

            cells[4, 0].PutValue(3);
            cells[4, 1].PutValue("Bob");
            cells[4, 2].PutValue(40);

            try
            {
                // Eliminar duplicados de las filas 1-4 (basado en 0), columnas 0-2
                // Comprobar duplicados basándose en las dos primeras columnas (ID y Nombre)
                cells.RemoveDuplicates(1, 0, 4, 2, true, new int[] { 0, 1 });

                Console.WriteLine("Duplicates removed successfully. Remaining rows: " + (cells.MaxDataRow + 1));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveDuplicates method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("RemoveDuplicatesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


