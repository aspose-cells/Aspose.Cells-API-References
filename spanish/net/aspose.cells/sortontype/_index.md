---
title: "Enumeración SortOnType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.SortOnType. Tipo de valor ordenado"
type: docs
url: /es/net/aspose.cells/sortontype/
---
## SortOnType enumeration

Tipo de valor ordenado.

```csharp
public enum SortOnType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Value | `0` | Ordena por el valor de las celdas. |
| CellColor | `1` | Ordena por el color de las celdas. |
| FontColor | `2` | Ordena por el color de fuente de las celdas. |
| Icon | `3` | Ordena por ícono condicional. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SortOnTypeDemo
    {
        public static void SortOnTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(95);
            worksheet.Cells["B4"].PutValue(75);

            // Aplicar filtro automático al rango
            worksheet.AutoFilter.Range = "A1:B4";

            // Obtener el filtro automático
            AutoFilter autoFilter = worksheet.AutoFilter;

            // Obtener el clasificador de datos
            DataSorter sorter = autoFilter.Sorter;

            // Establecer la primera clave para ordenar por los valores de la segunda columna (Puntuación)
            sorter.AddKey(1, SortOnType.Value, SortOrder.Descending, null);

            // Ordenar los datos en el rango
            sorter.Sort(worksheet.Cells, 1, 0, 3, 1);

            // Guarda el libro de trabajo
            workbook.Save("SortOnTypeExample.xlsx");

            // Genere la salida de los resultados
            Console.WriteLine("Data sorted by Score in descending order.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


