---
title: "Cells.ClearContents"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Cells method. Borra el contenido de un rango"
type: docs
url: /es/net/aspose.cells/cells/clearcontents/
---
## ClearContents(CellArea) {#clearcontents}

Borra el contenido de un rango.

```csharp
public void ClearContents(CellArea range)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | CellArea | Rango a eliminar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearContentsWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Poblar algunos datos en un área de celdas
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 2;
            area.EndColumn = 2;

            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Data_{row}_{col}");
                }
            }

            Console.WriteLine("Before ClearContents:");
            PrintCellAreaContents(cells, area);

            // Borrar el contenido del área de celdas
            cells.ClearContents(area);

            Console.WriteLine("\nAfter ClearContents:");
            PrintCellAreaContents(cells, area);
        }

        private static void PrintCellAreaContents(Cells cells, CellArea area)
        {
            for (int row = area.StartRow; row <= area.EndRow; row++)
            {
                for (int col = area.StartColumn; col <= area.EndColumn; col++)
                {
                    Console.Write(cells[row, col].StringValue + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearContents(int, int, int, int) {#clearcontents_1}

Borra el contenido de un rango.

```csharp
public void ClearContents(int startRow, int startColumn, int endRow, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | Índice de fila inicial. |
| startColumn | Int32 | Índice de columna inicial. |
| endRow | Int32 | Índice de fila final. |
| endColumn | Int32 | Índice de columna final. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearContentsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Rellene algunas celdas con valores
            cells[0, 0].PutValue("Value A1");
            cells[0, 1].PutValue("Value B1");
            cells[1, 0].PutValue("Value A2");
            cells[1, 1].PutValue("Value B2");

            // Mostrar valores originales
            Console.WriteLine("Before ClearContents:");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Borrar el contenido de las celdas en el rango (0,1) a (1,1)
            cells.ClearContents(0, 1, 1, 1);

            // Mostrar valores después de borrar
            Console.WriteLine("\nAfter ClearContents(0, 1, 1, 1):");
            Console.WriteLine("A1: " + cells[0, 0].StringValue);
            Console.WriteLine("B1: " + cells[0, 1].StringValue);
            Console.WriteLine("A2: " + cells[1, 0].StringValue);
            Console.WriteLine("B2: " + cells[1, 1].StringValue);

            // Guarda el libro de trabajo
            workbook.Save("ClearContentsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


