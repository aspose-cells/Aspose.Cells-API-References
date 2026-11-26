---
title: "RowCollection.GetEnumerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método RowCollection. Obtiene un enumerador que recorre filas a través de esta colección"
type: docs
url: /es/net/aspose.cells/rowcollection/getenumerator/
---
## GetEnumerator() {#getenumerator}

Obtiene un enumerador que recorre las filas de esta colección

```csharp
public IEnumerator GetEnumerator()
```

### Valor de retorno

El enumerador de filas que recorrerá todas las filas existentes en esta colección.

### Ejemplos

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer alturas de fila para la demostración
            worksheet.Cells.SetRowHeight(0, 15);
            worksheet.Cells.SetRowHeight(1, 20);
            worksheet.Cells.SetRowHeight(2, 25);

            IEnumerator enumerator = worksheet.Cells.Rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine($"Row index: {row.Index}, Height: {row.Height}");
            }
        }
    }
}
```

### Ver también

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Obtiene un enumerador que recorre las filas de esta colección

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| invertido | Booleano | si enumerar filas en orden invertido |
| sync | Booleano | si el enumerador devuelto debe comprobar la modificación de la colección de filas y mantenerse sincronizado con ella. |

### Valor de retorno

El enumerador de filas que recorrerá todas las filas existentes en esta colección.

### Observaciones

Si la colección de filas se modifica (por operaciones que pueden causar que se instancie una nueva Row o que se elimine una Row existente) durante el recorrido con el enumerador, se debe usar el enumerador sincronizado en lugar del enumerador normal para que el recorrido pueda continuar desde la posición justo después de la que fue recorrida por el último MoveNext(). Sin embargo, junto con la ventaja de que no se omita ni recorra repetidamente ningún elemento, la desventaja del enumerador sincronizado es que el rendimiento se degradará un poco al compararlo con el enumerador normal.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo a las filas
            for (int i = 0; i < 5; i++)
            {
                Row row = worksheet.Cells.Rows[i];
                row[0].PutValue($"Row {i + 1}");
            }
            
            try
            {
                // Obtener la RowCollection
                RowCollection rows = worksheet.Cells.Rows;
                
                // Llamar a GetEnumerator con los parámetros (reversed: true, sync: false)
                IEnumerator enumerator = rows.GetEnumerator(true, false);
                
                Console.WriteLine("Iterating rows in reverse order:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
                
                // Llamar a GetEnumerator con los parámetros (reversed: false, sync: true)
                enumerator = rows.GetEnumerator(false, true);
                
                Console.WriteLine("\nIterating rows in normal order (synchronized):");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("RowCollectionGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


