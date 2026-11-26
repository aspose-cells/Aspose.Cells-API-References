---
title: "Cells.Merge"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Fusiona un rango especificado de celdas en una sola celda"
type: docs
url: /es/net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

Fusiona un rango especificado de celdas en una sola celda.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila de este rango(basado en cero) |
| firstColumn | Int32 | Primera columna de este rango(basado en cero) |
| totalRows | Int32 | Número de filas(basado en uno) |
| totalColumns | Int32 | Número de columnas(basado en uno) |

### Observaciones

Referencia la celda fusionada mediante la dirección de la celda superior izquierda del rango.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Coloca valores en celdas para demostrar la fusión
            cells[0, 0].PutValue("Merged Area");
            cells[5, 5].PutValue("Not Merged");

            // Fusiona celdas comenzando desde la fila 0, columna 0 abarcando 3 filas y 2 columnas
            cells.Merge(0, 0, 3, 2);

            // Guarda el libro de trabajo
            workbook.Save("MergeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

Fusiona un rango especificado de celdas en una sola celda.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila de este rango(basado en cero) |
| firstColumn | Int32 | Primera columna de este rango(basado en cero) |
| totalRows | Int32 | Número de filas(basado en uno) |
| totalColumns | Int32 | Número de columnas(basado en uno) |
| mergeConflict | Booleano | Conflicto de fusión en rangos fusionados. |

### Observaciones

Referencia la celda fusionada mediante la dirección de la celda superior izquierda del rango. Si mergeConflict es verdadero y el rango fusionado entra en conflicto con otras celdas fusionadas, esas otras celdas fusionadas se eliminarán automáticamente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fusiona celdas desde la fila 3, columna 4 (D3) hasta la fila 7, columna 5 (E7) - 5 filas y 2 columnas
            worksheet.Cells.Merge(3, 4, 5, 2, true);
            
            // Guarda el libro de trabajo
            workbook.Save("MergeDemoOutput.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

Fusiona un rango especificado de celdas en una sola celda.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila de este rango(basado en cero) |
| firstColumn | Int32 | Primera columna de este rango(basado en cero) |
| totalRows | Int32 | Número de filas(basado en uno) |
| totalColumns | Int32 | Número de columnas(basado en uno) |
| checkConflict | Booleano | Indica si la comprobación de que las celdas fusionadas intersectan otras celdas fusionadas |
| mergeConflict | Booleano | Conflicto de fusión en rangos fusionados. |

### Observaciones

Referencia la celda fusionada mediante la dirección de la celda superior izquierda del rango. Si mergeConflict es verdadero y el rango fusionado entra en conflicto con otras celdas fusionadas, esas otras celdas fusionadas se eliminarán automáticamente.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanBooDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Coloca algunos datos en celdas para ser fusionadas
            cells[0, 1].PutValue("Merged Cell");
            cells[1, 1].PutValue("This will be merged");

            // Fusiona celdas sin opciones (fusión simple)
            cells.Merge(0, 1, 2, 2);
            Console.WriteLine("Cells merged without options");

            // Desfusiona primero para demostrar la siguiente fusión
            cells.UnMerge(0, 1, 2, 2);

            // Fusiona celdas con ignoreStyle=false y mergeConflict=true
            cells.Merge(0, 1, 2, 2, false, true);
            Console.WriteLine("Cells merged with ignoreStyle=false and mergeConflict=true");

            // Guarda el libro de trabajo
            workbook.Save("MergeCellsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


