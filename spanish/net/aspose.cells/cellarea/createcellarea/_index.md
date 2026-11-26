---
title: "CellArea.CreateCellArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellArea. Crea un área de celda"
type: docs
url: /es/net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

Crea un área de celdas.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | La fila de inicio. |
| startColumn | Int32 | La columna de inicio. |
| endRow | Int32 | La fila final. |
| endColumn | Int32 | La columna final. |

### Valor de retorno

Devuelve un [`CellArea`](../).

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Rellenar celdas con datos de ejemplo
            int[] values = { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
            for (int i = 0; i < values.Length; i++)
            {
                cells[i, i / 3].PutValue(values[i]);
            }

            // Crear y configurar el clasificador de datos
            DataSorter sorter = wb.DataSorter;
            sorter.Clear();
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 2;
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1;
            sorter.Order3 = SortOrder.Ascending;
            sorter.Key3 = 0;

            // Ordenar usando CreateCellArea con parámetros Int32
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));

            // Salida de valores ordenados
            Console.WriteLine("Sorted values:");
            for (int i = 0; i < 9; i++)
            {
                Console.WriteLine(cells[i, 2 - i / 3].IntValue);
            }
        }
    }
}
```

### Ver también

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

Crea un área de celdas.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startCellName | String | La celda superior izquierda del rango. |
| endCellName | String | La celda inferior derecha del rango. |

### Valor de retorno

Devuelve un [`CellArea`](../).

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Poblar algunos datos en la columna A
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Data {i}");
            }

            // Crear área de celdas desde B1 hasta B10
            CellArea area = CellArea.CreateCellArea("B1", "B10");
            
            // Insertar rango desplazando las celdas hacia abajo
            cells.InsertRange(area, ShiftType.Down);
            
            // Verificar la operación comprobando los valores de las celdas
            Console.WriteLine("Inserted range from B1 to B10. Total rows: " + cells.Rows.Count);
        }
    }
}
```

### Ver también

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


