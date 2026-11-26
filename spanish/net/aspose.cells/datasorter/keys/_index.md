---
title: "DataSorter.Keys"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorter. Obtiene la lista de claves del ordenador de datos"
type: docs
url: /es/net/aspose.cells/datasorter/keys/
---
## DataSorter.Keys property

Obtiene la lista de claves del data sorter.

```csharp
public DataSorterKeyCollection Keys { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKeysDemo
    {
        public static void Run()
        {
            // Crear un objeto libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Inicializar el ordenamiento de datos
            DataSorter sorter = workbook.DataSorter;
            
            // Agregar clave de ordenación para la columna A (índice 0)
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordenar los datos
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Demostrar el uso de la propiedad Keys
            DataSorterKeyCollection keys = sorter.Keys;
            Console.WriteLine("Sort Keys Information:");
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Column Index: {key.Index}, Sort Order: {key.Order}");
            }

            // Guarda el libro de trabajo
            workbook.Save("DataSorterKeysDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


