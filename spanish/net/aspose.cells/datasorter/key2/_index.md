---
title: "DataSorter.Key2"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorter. Representa el índice de la segunda columna ordenada; posición absoluta, la columna A es 0, B es 1"
type: docs
url: /es/net/aspose.cells/datasorter/key2/
---
## DataSorter.Key2 property

Representa el índice de la segunda columna ordenada (posición absoluta, la columna A es 0, B es 1, ...).

```csharp
public int Key2 { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey2Demo
    {
        public static void Run()
        {
            // Crea un libro y añade datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Crear DataSorter y establecer propiedades
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;
            sorter.Key1 = 0; // Sort by first column (Name)
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key2 = 1; // Then sort by second column (Age)
            sorter.Order2 = SortOrder.Descending;

            // Ordenar el rango de datos
            sorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Mostrar los datos ordenados para demostrar el uso de Key2
            Console.WriteLine("Sorted Data:");
            for (int i = 0; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[i, 0].StringValue} - {worksheet.Cells[i, 1].IntValue}");
            }
        }
    }
}
```

### Ver también

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


