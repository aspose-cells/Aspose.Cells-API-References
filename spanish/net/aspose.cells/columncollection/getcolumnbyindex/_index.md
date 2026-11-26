---
title: "ColumnCollection.GetColumnByIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ColumnCollection. Obtiene el objeto Column por la posición en la lista"
type: docs
url: /es/net/aspose.cells/columncollection/getcolumnbyindex/
---
## ColumnCollection.GetColumnByIndex method

Obtiene el objeto [`Column`](../../column/) por la posición en la lista.

```csharp
public Column GetColumnByIndex(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | La posición en la lista. |

### Valor de retorno

Devuelve el objeto column.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetColumnByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la columna A
            worksheet.Cells["A1"].Value = "Aspose.Cells Column Demo";

            try
            {
                // Obtener referencia a la colección de columnas
                ColumnCollection columns = worksheet.Cells.Columns;

                // Acceder a la columna en el índice 0 (columna A) usando GetColumnByIndex
                Column column = columns.GetColumnByIndex(0);

                // Modificar el ancho de la columna para demostrar el acceso a columnas
                column.Width = 25;

                Console.WriteLine("Modified width of column at index 0 (Column A) to 25 characters.");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid column index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("ColumnCollectionMethodGetColumnByIndexWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


