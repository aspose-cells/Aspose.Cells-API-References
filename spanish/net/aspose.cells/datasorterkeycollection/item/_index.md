---
title: "DataSorterKeyCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorterKeyCollection. Obtiene y establece DataSorterKey por índice"
type: docs
url: /es/net/aspose.cells/datasorterkeycollection/item/
---
## DataSorterKeyCollection indexer

Obtiene y establece [`DataSorterKey`](../../datasorterkey/) por índice.

```csharp
public DataSorterKey this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class DataSorterKeyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["B4"].PutValue(78);

            // Crear un objeto lista (tabla)
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[index];

            // Agregar clave de ordenación (ordenar por la columna Score en orden descendente)
            table.AutoFilter.Sorter.AddKey(1, SortOrder.Descending);
            table.AutoFilter.Sorter.Sort();

            // Demostrar el uso de la propiedad Item
            DataSorterKey key = table.AutoFilter.Sorter.Keys[0];
            Console.WriteLine("Sort Key Index: {0}, Order: {1}", key.Index, key.Order);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [DataSorterKey](../../datasorterkey/)
* class [DataSorterKeyCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


