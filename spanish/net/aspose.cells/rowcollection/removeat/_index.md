---
title: "RowCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método RowCollection. Elimina el elemento de fila en la posición de índice especificada en esta colección"
type: docs
url: /es/net/aspose.cells/rowcollection/removeat/
---
## RowCollection.RemoveAt method

Eliminar el elemento de fila en el índice (posición) especificado en esta colección.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index | Int32 | índice basado en cero (posición, no [`Index`](../../row/index/)) del elemento de fila existente en esta colección. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a las celdas en las primeras filas
            worksheet.Cells["A1"].PutValue("Row 1");
            worksheet.Cells["A2"].PutValue("Row 2");
            worksheet.Cells["A3"].PutValue("Row 3");
            worksheet.Cells["A4"].PutValue("Row 4");

            // Mostrar el recuento inicial de filas
            Console.WriteLine($"Initial row count: {worksheet.Cells.Rows.Count}");

            try
            {
                // Llamar al método RemoveAt para eliminar la fila en el índice 1 (segunda fila)
                worksheet.Cells.Rows.RemoveAt(1);

                Console.WriteLine("Method executed successfully. Row at index 1 removed.");

                // Mostrar el recuento actualizado de filas
                Console.WriteLine($"Updated row count: {worksheet.Cells.Rows.Count}");

                // Mostrar el efecto - La fila 2 debe ser eliminada, la fila 3 pasa a ser la fila 2
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("RowCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


