---
title: "DataSorter.Sort"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DataSorter. Ordena los datos del área"
type: docs
url: /es/net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Ordena los datos del área.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| celdas | Celdas | Las celdas contienen el área de datos. |
| startRow | Int32 | La fila inicial del área. |
| startColumn | Int32 | La columna inicial del área. |
| endRow | Int32 | La fila final del área. |
| endColumn | Int32 | La columna final del área. |

### Valor de retorno

Los índices originales (posición absoluta, por ejemplo, la columna A es 0, B es 1, ...) de las filas/columnas ordenadas. Si no se necesita mover ninguna fila/columna con esta operación de ordenación, se devolverá null.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Rellene datos de ejemplo
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue(6 - i);
            }
            
            // Ocultar una fila para demostrar la ordenación con filas ocultas
            cells.Rows[1].IsHidden = true;
            
            // Crear y configurar el sorter
            DataSorter sorter = wb.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Demostrar el método Sort con Cells y parámetros Int32
            sorter.Sort(cells, 0, 0, 5, 0);
            
            // Mostrar resultados en la consola
            for (int i = 0; i < 6; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {cells[i, 0].IntValue}");
            }
            Console.WriteLine($"Is row 2 hidden? {cells.Rows[1].IsHidden}");
        }
    }
}
```

### Ver también

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Ordenar los datos del área.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| celdas | Celdas | Las celdas contienen el área de datos. |
| área | CellArea | El área necesaria para ordenar |

### Valor de retorno

Los índices originales (posición absoluta, por ejemplo, la columna A es 0, B es 1, ...) de las filas/columnas ordenadas. Si no se necesita mover ninguna fila/columna con esta operación de ordenación, se devolverá null.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortWithCellsCellAreaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(1995);
            worksheet.Cells["B2"].PutValue(10000);
            worksheet.Cells["A3"].PutValue(1996);
            worksheet.Cells["B3"].PutValue(15000);
            worksheet.Cells["A4"].PutValue(1997);
            worksheet.Cells["B4"].PutValue(12000);
            worksheet.Cells["A5"].PutValue(1998);
            worksheet.Cells["B5"].PutValue(18000);

            // Crear un clasificador de datos
            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.HasHeaders = true;
            dataSorter.Key1 = 0; // Sort by first column (Year)
            dataSorter.Order1 = SortOrder.Descending;

            // Definir área de ordenación
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 1;

            // Ejecutar ordenación
            dataSorter.Sort(worksheet.Cells, area);

            // Guarda el libro de trabajo
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Ordenar los datos en el rango.

```csharp
public int[] Sort()
```

### Valor de retorno

Los índices originales (posición absoluta, por ejemplo, la columna A es 0, B es 1, ...) de las filas/columnas ordenadas. Si no se necesita mover ninguna fila/columna con esta operación de ordenación, se devolverá null.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodSortDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para ordenar
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("C");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["B4"].PutValue(20);

            // Crear un objeto tabla/lista
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Ordenar los datos por la primera columna
            table.AutoFilter.Sorter.Sort();

            // Guarda el libro de trabajo
            workbook.Save("SortedData.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


