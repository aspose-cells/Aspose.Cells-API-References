---
title: "Cells.DeleteColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina varias columnas"
type: docs
url: /es/net/aspose.cells/cells/deletecolumns/
---
## DeleteColumns(int, int, bool) {#deletecolumns_1}

Elimina varias columnas.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | Índice de la primera columna a eliminar. |
| totalColumns | Int32 | Cantidad de columnas a eliminar. |
| updateReference | Booleano | Indica si se actualizan referencias en otras hojas de cálculo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // Agregar una fórmula que haga referencia a estas columnas
            worksheet.Cells["D1"].Formula = "=SUM(A2:C2)";

            Console.WriteLine("Before deleting columns:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1: " + worksheet.Cells["C1"].Value);
            Console.WriteLine("D1 formula: " + worksheet.Cells["D1"].Formula);

            // Eliminar la columna B (índice 1) y desplazar las columnas restantes a la izquierda
            worksheet.Cells.DeleteColumns(1, 1, true);

            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("C1 formula: " + worksheet.Cells["C1"].Formula);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteColumns(int, int, DeleteOptions) {#deletecolumns}

Elimina varias columnas.

```csharp
public void DeleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | Índice de la primera columna a eliminar. |
| totalColumns | Int32 | Cantidad de columnas a eliminar. |
| opciones | DeleteOptions | Opciones para la operación de eliminación |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodDeleteColumnsWithInt32Int32DeleteOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar datos de ejemplo en las columnas A-E
            for (int col = 0; col < 5; col++)
            {
                worksheet.Cells[0, col].Value = $"Column {(char)('A' + col)}";
                worksheet.Cells[1, col].Value = $"Data{col + 1}";
            }

            // Crear DeleteOptions y configurar los ajustes
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Update references in other cells
            };

            try
            {
                // Eliminar 2 columnas comenzando desde la columna B (índice 1)
                worksheet.Cells.DeleteColumns(1, 2, options);
                
                Console.WriteLine("Deleted columns B and C successfully");
                
                // Mostrar los datos restantes en la columna B (columna D original)
                Console.WriteLine($"New column B value: {worksheet.Cells[1, 1].StringValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteColumns: {ex.Message}");
            }
            
            // Guardar el libro de trabajo modificado
            workbook.Save("DeleteColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


