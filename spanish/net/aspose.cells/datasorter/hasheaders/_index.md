---
title: "DataSorter.HasHeaders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataSorter. Representa si el rango tiene encabezados"
type: docs
url: /es/net/aspose.cells/datasorter/hasheaders/
---
## DataSorter.HasHeaders property

Representa si el rango tiene encabezados.

```csharp
public bool HasHeaders { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyHasHeadersDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar encabezados y datos de muestra
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["B4"].PutValue(12);

            // Crear un DataSorter y establecer HasHeaders a true
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true; // This tells the sorter the first row contains headers
            
            // Ordenar por la primera columna (Frutas) en orden ascendente
            sorter.AddKey(0, SortOrder.Ascending);
            
            // Ordenar el rango de datos (incluyendo encabezados)
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "B4"));

            // Guardar el libro de trabajo ordenado
            workbook.Save("SortedWithHeaders.xlsx");
        }
    }
}
```

### Ver también

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


