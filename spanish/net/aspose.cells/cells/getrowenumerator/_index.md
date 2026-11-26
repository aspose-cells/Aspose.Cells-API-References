---
title: "Cells.GetRowEnumerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el enumerador de filas"
type: docs
url: /es/net/aspose.cells/cells/getrowenumerator/
---
## Cells.GetRowEnumerator method

Obtiene el enumerador de filas.

```csharp
[Obsolete("Use RowCollection.GetEnumerator() method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetRowEnumerator()
```

### Valor de retorno

El enumerador de filas.

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método RowCollection.GetEnumerator(). Este método será eliminado 12 meses después desde mayo de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetRowEnumeratorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Row 1 Data");
            worksheet.Cells["A3"].PutValue("Row 3 Data");
            worksheet.Cells["A5"].PutValue("Row 5 Data");

            try
            {
                // Obtener el enumerador de filas de la colección Cells
                IEnumerator enumerator = worksheet.Cells.GetRowEnumerator();
                
                Console.WriteLine("Iterating through rows containing data:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Cell cell = row.GetCellOrNull(0); // Get first cell in row
                    string cellValue = cell != null ? cell.Value.ToString() : "empty";
                    Console.WriteLine($"Row {row.Index}: First cell value = {cellValue}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowEnumerator method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("MethodGetRowEnumeratorDemo.xlsx");
        }
    }
}
```

### Ver también

* method [GetEnumerator](../../rowcollection/getenumerator/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


