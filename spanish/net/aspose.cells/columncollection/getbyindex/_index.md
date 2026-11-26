---
title: "ColumnCollection.GetByIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ColumnCollection. Obtiene el objeto column por el índice"
type: docs
url: /es/net/aspose.cells/columncollection/getbyindex/
---
## ColumnCollection.GetByIndex method

Obtiene el objeto column por el índice.

```csharp
[Obsolete("Use Columns.GetColumnByIndex() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Column GetByIndex(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 |  |

### Valor de retorno

Devuelve el objeto column.

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método Columns.GetColumnByIndex(). Esta propiedad será eliminada 12 meses después desde junio de 2010. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree columnas en la colección estableciendo anchos
            worksheet.Cells.Columns[0].Width = 15;  // Column 0
            worksheet.Cells.Columns[2].Width = 20;  // Column 2
            worksheet.Cells.Columns[4].Width = 25;  // Column 4

            try
            {
                // Obtenga la segunda columna de ColumnCollection (índice 1)
                Column column = worksheet.Cells.Columns.GetByIndex(1);

                Console.WriteLine($"Retrieved column at collection index 1");
                Console.WriteLine($"Worksheet column index: {column.Index}");
                Console.WriteLine($"Original width: {column.Width}");

                // Modifique la columna recuperada
                column.Width = 35;
                Console.WriteLine($"Updated width: {column.Width}");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ColumnCollectionGetByIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


