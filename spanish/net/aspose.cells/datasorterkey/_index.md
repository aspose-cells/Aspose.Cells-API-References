---
title: "Clase DataSorterKey"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DataSorterKey. Representa la clave del clasificador de datos"
type: docs
url: /es/net/aspose.cells/datasorterkey/
---
## DataSorterKey class

Representa la clave del ordenador de datos.

```csharp
public class DataSorterKey
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Color](../../aspose.cells/datasorterkey/color/) { get; } | Obtiene el color ordenado. |
| [IconId](../../aspose.cells/datasorterkey/iconid/) { get; } | Representa el id del tipo de conjunto de íconos. |
| [IconSetType](../../aspose.cells/datasorterkey/iconsettype/) { get; } | Representa el tipo de conjunto de íconos. |
| [Index](../../aspose.cells/datasorterkey/index/) { get; } | Obtiene el índice de columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [Order](../../aspose.cells/datasorterkey/order/) { get; } | Indica el orden de clasificación. |
| [Type](../../aspose.cells/datasorterkey/type/) { get; } | Representa el tipo de clasificación. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataSorterKeyDemo
    {
        public static void DataSorterKeyExample()
        {
            // Crea un objeto de libro de trabajo y carga un archivo de plantilla
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos de muestra para ordenar
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Instancia un objeto clasificador de datos
            DataSorter sorter = workbook.DataSorter;

            // Agrega la clave para la primera columna (A) para ordenar en orden ascendente
            sorter.AddKey(0, SortOrder.Ascending);

            // Crea un área de celdas (rango) para ordenar
            CellArea ca = CellArea.CreateCellArea("A1", "A5");

            // Ejecuta la ordenación
            sorter.Sort(worksheet.Cells, ca);

            // Guarda el archivo de salida
            workbook.Save("DataSorterKeyExample.xlsx");
            workbook.Save("DataSorterKeyExample.pdf");

            // Acceda a DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Itera a través de las claves e imprime sus propiedades
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Order: {key.Order}");
                Console.WriteLine($"Index: {key.Index}");
                Console.WriteLine($"Type: {key.Type}");
                Console.WriteLine($"IconSetType: {key.IconSetType}");
                Console.WriteLine($"IconId: {key.IconId}");
                Console.WriteLine($"Color: {key.Color}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


