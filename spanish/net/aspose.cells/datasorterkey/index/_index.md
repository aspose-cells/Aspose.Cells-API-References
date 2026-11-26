---
title: "DataSorterKey.Index"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorterKey. Obtiene el índice de columna ordenada, posición absoluta (la columna A es 0, B es 1)"
type: docs
url: /es/net/aspose.cells/datasorterkey/index/
---
## DataSorterKey.Index property

Obtiene el índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

```csharp
public int Index { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIndexDemo
    {
        public static void Run()
        {
            // Crear un objeto libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para ordenar
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Crea un clasificador de datos y agrega una clave de ordenación
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordenar los datos
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Demuestra el uso de la propiedad Index
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Column index being sorted: {key.Index}");
            }

            // Guardar el resultado
            workbook.Save("DataSorterKeyExample.xlsx");
        }
    }
}
```

### Ver también

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


