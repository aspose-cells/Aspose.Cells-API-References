---
title: "Clase RowCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.RowCollection. Recopila los objetos Row que representan las filas individuales en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/rowcollection/
---
## RowCollection class

Recopila los objetos [`Row`](../row/) que representan las filas individuales en una hoja de cálculo.

```csharp
public class RowCollection : IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells/rowcollection/count/) { get; } | Obtiene el número de filas en esta colección. |
| [Item](../../aspose.cells/rowcollection/item/) { get; } | Obtiene un objeto [`Row`](../row/) por el índice de fila dado. El objeto Row del índice de fila dado se instanciará si no existe previamente. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Clear](../../aspose.cells/rowcollection/clear/)() | Eliminar todas las filas y celdas. |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator)() | Obtiene un enumerador que recorre las filas de esta colección |
| [GetEnumerator](../../aspose.cells/rowcollection/getenumerator/#getenumerator_1)(bool, bool) | Obtiene un enumerador que recorre las filas de esta colección |
| [GetRowByIndex](../../aspose.cells/rowcollection/getrowbyindex/)(int) | Obtiene el objeto fila por la posición en la lista. |
| [RemoveAt](../../aspose.cells/rowcollection/removeat/)(int) | Eliminar el elemento de fila en el índice (posición) especificado en esta colección. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionDemo
    {
        public static void RowCollectionExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Obteniendo la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("Aspose.Cells");
            // Obtener la colección Rows
            RowCollection rows = worksheet.Cells.Rows;

            // Obtener el número de filas en la colección
            int rowCount = rows.Count;
            Console.WriteLine("Number of rows: " + rowCount);

            // Obtener la primera fila
            Row firstRow = rows[0];
            Console.WriteLine("First row index: " + firstRow.Index);

            // Iterar a través de las filas usando GetEnumerator
            IEnumerator enumerator = rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine("Row index: " + row.Index + ", Height: " + row.Height);
            }

            // Obtener una fila por índice
            Row specificRow = rows.GetRowByIndex(1);
            Console.WriteLine("Specific row index: " + specificRow.Index);

            // Eliminar todas las filas y celdas
            rows.Clear();
            Console.WriteLine("Rows cleared.");

            // Guarda el libro de trabajo
            workbook.Save("RowCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


