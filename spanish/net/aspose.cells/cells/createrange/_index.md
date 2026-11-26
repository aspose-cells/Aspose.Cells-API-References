---
title: "Cells.CreateRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Crea un objeto Range a partir de un rango de celdas"
type: docs
url: /es/net/aspose.cells/cells/createrange/
---
## CreateRange(string, string) {#createrange_3}

Crea un objeto [`Range`](../../range/) a partir de un rango de celdas.

```csharp
public Range CreateRange(string upperLeftCell, string lowerRightCell)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| upperLeftCell | String | Nombre de la celda superior izquierda. |
| lowerRightCell | String | Nombre de la celda inferior derecha. |

### Valor de retorno

Un objeto [`Range`](../../range/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Crea un rango de A1 a A2
            Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
            range.Name = "MyRange";
            
            // Establece valores en el rango
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            
            // Usa el rango en una fórmula
            cells["B1"].Formula = "=SUM(MyRange)";
            
            // Calcular la fórmula
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of MyRange (A1:A2) is: " + cells["B1"].IntValue);
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, int, int) {#createrange_1}

Crea un objeto [`Range`](../../range/) a partir de un rango de celdas.

```csharp
public Range CreateRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila de este rango |
| firstColumn | Int32 | Primera columna de este rango |
| totalRows | Int32 | Número de filas |
| totalColumns | Int32 | Número de columnas |

### Valor de retorno

Un objeto [`Range`](../../range/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea el rango de origen (fila inicial 2, columna 2 con 3 filas y 4 columnas)
            Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);

            // Rellena el rango de origen con datos de ejemplo
            for (int i = 0; i < rangeSrc.RowCount; i++)
            {
                for (int j = 0; j < rangeSrc.ColumnCount; j++)
                {
                    rangeSrc[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Crear rango de destino (fila inicial 8, columna 0 con las mismas dimensiones)
            Aspose.Cells.Range rangeDest = cells.CreateRange(8, 0, 3, 4);

            // Copiar valores del origen al destino
            rangeDest.CopyValue(rangeSrc);

            // Guarda el libro de trabajo
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(string) {#createrange_2}

Crea un objeto [`Range`](../../range/) a partir de una dirección del rango.

```csharp
public Range CreateRange(string address)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| address | String | La dirección del rango. |

### Valor de retorno

Un objeto [`Range`](../../range/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango usando una dirección de cadena
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Rellenar datos en el rango
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Crear otro rango en una nueva hoja de cálculo
            workbook.Worksheets.Add();
            Worksheet worksheet2 = workbook.Worksheets[1];
            Aspose.Cells.Range range2 = worksheet2.Cells.CreateRange("A1:C3");

            // Copiar datos entre rangos
            range2.Copy(range);

            // Guarda el libro de trabajo
            workbook.Save("CreateRangeWithStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, bool) {#createrange}

Crea un objeto [`Range`](../../range/) a partir de filas de celdas o columnas de celdas.

```csharp
public Range CreateRange(int firstIndex, int number, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | Int32 | Índice de la primera fila o índice de la primera columna, basado en cero. |
| número | Int32 | Número total de filas o columnas, basado en uno. |
| isVertical | Booleano | Verdadero - Rango creado a partir de columnas de celdas. Falso - Rango creado a partir de filas de celdas. |

### Valor de retorno

Un objeto [`Range`](../../range/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear un rango que comienza en la celda A1 (0,0) con 5 filas y 3 columnas
            Aspose.Cells.Range range = cells.CreateRange(0, 0, true);

            // Rellenar algunos datos en el rango
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Row {i}, Col {j}");
                }
            }

            // Guarda el libro de trabajo
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


