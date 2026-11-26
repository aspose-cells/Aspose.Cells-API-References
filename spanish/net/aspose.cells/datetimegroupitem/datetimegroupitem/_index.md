---
title: "DateTimeGroupItem.DateTimeGroupItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de DateTimeGroupItem."
type: docs
url: /es/net/aspose.cells/datetimegroupitem/datetimegroupitem/
---
## DateTimeGroupItem constructor

```csharp
public DateTimeGroupItem(DateTimeGroupingType type, int year, int month, int day, int hour, 
    int minute, int second)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | DateTimeGroupingType |  |
| año | Int32 |  |
| mes | Int32 |  |
| día | Int32 |  |
| hora | Int32 |  |
| minuto | Int32 |  |
| segundo | Int32 |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemMethodCtorWithDateTimeGroupingTypeInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de datetime de muestra a la columna A
            worksheet.Cells["A1"].PutValue("Order Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 3, 15, 9, 30, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 4, 20, 14, 15, 45));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 25, 10, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2024, 3, 1, 8, 45, 30));

            // Aplicar autofiltro a la columna de fechas
            worksheet.AutoFilter.Range = "A1:A5";

            try
            {
                // Crear DateTimeGroupItem para el agrupamiento de marzo 2023
                DateTimeGroupItem groupItem = new DateTimeGroupItem(
                    DateTimeGroupingType.Month, // Group by Month
                    2023,   // Year
                    3,      // Month (March)
                    1,      // Day (ignored in Month grouping)
                    0,      // Hour
                    0,      // Minute
                    0       // Second
                );

                // Configurar el filtro para mostrar fechas de marzo 2023
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.MultipleFilters;
                filterColumn.Filter = groupItem;

                // Actualizar el filtro para aplicar los cambios
                worksheet.AutoFilter.Refresh();

                Console.WriteLine("DateTimeGroupItem created and filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying date filter: {ex.Message}");
            }

            // Guardar el libro de trabajo filtrado
            workbook.Save("DateTimeGroupItemConstructorDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


