---
title: "Clase DataSorter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DataSorter. Descripción resumida de DataSorter"
type: docs
url: /es/net/aspose.cells/datasorter/
---
## DataSorter class

Descripción resumida para DataSorter.

```csharp
public class DataSorter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive/) { get; set; } | Obtiene y establece si es sensible a mayúsculas al comparar cadenas. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders/) { get; set; } | Representa si el rango tiene encabezados. |
| [Key1](../../aspose.cells/datasorter/key1/) { get; set; } | Representa el índice de la primera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2/) { get; set; } | Representa el índice de la segunda columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3/) { get; set; } | Representa el índice de la tercera columna ordenada (posición absoluta, la columna A es 0, B es 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys/) { get; } | Obtiene la lista de claves del data sorter. |
| [Order1](../../aspose.cells/datasorter/order1/) { get; set; } | Representa el orden de clasificación de la primera clave. |
| [Order2](../../aspose.cells/datasorter/order2/) { get; set; } | Representa el orden de clasificación de la segunda clave. |
| [Order3](../../aspose.cells/datasorter/order3/) { get; set; } | Representa el orden de clasificación de la tercera clave. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber/) { get; set; } | Indica si se ordena cualquier cosa que parezca un número. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright/) { get; set; } | True indica que la orientación de ordenación es de izquierda a derecha. False indica que la orientación de ordenación es de arriba a abajo. El valor predeterminado es false. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddColorKey](../../aspose.cells/datasorter/addcolorkey/)(int, SortOnType, SortOrder, Color) | Agrega una clave de ordenación por color. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_1)(int, SortOrder) | Agrega el índice de columna ordenada y el orden de clasificación. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_2)(int, SortOrder, string) | Agrega el índice de columna ordenado y el orden de clasificación con una lista de clasificación personalizada. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_3)(int, SortOrder, string[]) | Agrega el índice de columna ordenado y el orden de clasificación con una lista de clasificación personalizada. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey)(int, SortOnType, SortOrder, object) | Agrega el índice de columna ordenado y el orden de clasificación con una lista de clasificación personalizada. |
| [Clear](../../aspose.cells/datasorter/clear/)() | Borrar todas las configuraciones. |
| [Sort](../../aspose.cells/datasorter/sort/#sort)() | Ordenar los datos en el rango. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_1)(Cells, CellArea) | Ordenar los datos del área. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_2)(Cells, int, int, int, int) | Ordena los datos del área. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterDemo
    {
        public static void DataSorterExample()
        {
            // Instanciar un nuevo objeto Workbook
            Workbook workbook = new Workbook("DataSorter_original.xlsx");

            // Obtener el objeto DataSorter del libro de trabajo
            DataSorter sorter = workbook.DataSorter;

            // Establecer el primer orden para el objeto DataSorter
            sorter.Order1 = SortOrder.Descending;
            // Definir la primera clave
            sorter.Key1 = 0;

            // Establecer el segundo orden para el objeto DataSorter
            sorter.Order2 = SortOrder.Ascending;
            // Definir la segunda clave
            sorter.Key2 = 1;

            // Crear un área de celdas (rango)
            CellArea ca = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 13,
                EndColumn = 1
            };

            // Ordenar datos en el rango de datos especificado (A1:B14)
            sorter.Sort(workbook.Worksheets[0].Cells, ca);

            // Guardar el archivo Excel
            workbook.Save("DataSorterExample.xlsx");
            workbook.Save("DataSorterExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


