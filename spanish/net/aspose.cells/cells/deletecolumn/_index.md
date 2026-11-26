---
title: "Cells.DeleteColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina una columna"
type: docs
url: /es/net/aspose.cells/cells/deletecolumn/
---
## DeleteColumn(int, bool) {#deletecolumn_1}

Elimina una columna.

```csharp
public void DeleteColumn(int columnIndex, bool updateReference)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | Índice de la columna a eliminar. |
| updateReference | Booleano | Indica si se actualizan referencias en otras hojas de cálculo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Rellena algunos datos de ejemplo en celdas
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }
            
            Console.WriteLine("Before deleting column:");
            PrintCellValues(sheet);
            
            // Elimina la primera columna y desplaza las columnas restantes a la izquierda
            sheet.Cells.DeleteColumn(0, true);
            
            Console.WriteLine("\nAfter deleting column 0:");
            PrintCellValues(sheet);
            
            // Guarda el libro de trabajo
            workbook.Save("DeleteColumnDemo.xlsx");
        }
        
        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    Console.Write(sheet.Cells[i, j].Value + "\t");
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

## DeleteColumn(int) {#deletecolumn}

Elimina una columna.

```csharp
public void DeleteColumn(int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | Índice de la columna a eliminar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Rellena algunos datos de ejemplo en columnas
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // Eliminar columna en el índice 1 (Columna B)
            cells.DeleteColumn(1);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Column deleted successfully.");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


