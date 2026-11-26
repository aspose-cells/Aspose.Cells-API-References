---
title: "DataSorter.CaseSensitive"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorter. Obtiene y establece si es sensible a mayúsculas al comparar cadenas"
type: docs
url: /es/net/aspose.cells/datasorter/casesensitive/
---
## DataSorter.CaseSensitive property

Obtiene y establece si es sensible a mayúsculas al comparar cadenas.

```csharp
public bool CaseSensitive { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Crea un libro de trabajo y una hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de muestra con variaciones de mayúsculas y minúsculas
            cells["A1"].PutValue("apple");
            cells["A2"].PutValue("Orange");
            cells["A3"].PutValue("banana");
            cells["A4"].PutValue("APPLE");
            cells["A5"].PutValue("orange");
            cells["A6"].PutValue("Banana");

            // Crear un clasificador de datos
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 0; // Sort by first column
            sorter.Order1 = SortOrder.Ascending;

            // Demostrar ordenación sensible a mayúsculas
            Console.WriteLine("Sorting with CaseSensitive = true:");
            sorter.CaseSensitive = true;
            sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
            PrintSortedData(cells, "A1:A6");

            // Demostrar ordenación insensible a mayúsculas
            Console.WriteLine("\nSorting with CaseSensitive = false:");
            sorter.CaseSensitive = false;
            sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
            PrintSortedData(cells, "A1:A6");
        }

        private static void PrintSortedData(Cells cells, string range)
        {
            Console.WriteLine("Sorted data:");
            foreach (Cell cell in cells.CreateRange(range))
            {
                Console.WriteLine(cell.StringValue);
            }
        }
    }
}
```

### Ver también

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


