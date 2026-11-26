---
title: "DataSorter.SortAsNumber"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorter. Indica si se ordena cualquier cosa que parezca un número"
type: docs
url: /es/net/aspose.cells/datasorter/sortasnumber/
---
## DataSorter.SortAsNumber property

Indica si se ordena cualquier cosa que parezca un número.

```csharp
public bool SortAsNumber { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortAsNumberDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con números mezclados y números en texto
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Crear área de celdas para ordenar
            CellArea ca = CellArea.CreateCellArea("A1", "A4");

            // Crear un clasificador de datos
            DataSorter sorter = workbook.DataSorter;
            int idx = CellsHelper.ColumnNameToIndex("A");

            // Agregar clave de ordenación (columna A)
            sorter.AddKey(idx, SortOrder.Ascending);

            // Ordenar como números (true) o como cadenas (false)
            sorter.SortAsNumber = true;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("Sorted as numbers:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Restablecer datos para la segunda ordenación
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // Ordenar como cadenas
            sorter.SortAsNumber = false;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("\nSorted as strings:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Ver también

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


