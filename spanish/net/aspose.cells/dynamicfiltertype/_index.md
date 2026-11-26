---
title: "Enum DynamicFilterType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.DynamicFilterType. Tipo de filtro dinámico"
type: docs
url: /es/net/aspose.cells/dynamicfiltertype/
---
## DynamicFilterType enumeration

Tipo de filtro dinámico.

```csharp
public enum DynamicFilterType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| AboveAverage | `0` | Muestra valores que están por encima del promedio. |
| BelowAverage | `1` | Muestra valores que están por debajo del promedio. |
| LastMonth | `2` | Muestra las fechas del mes pasado. |
| LastQuarter | `3` | Muestra las fechas del último trimestre. |
| LastWeek | `4` | Muestra las fechas de la semana pasada. |
| LastYear | `5` | Muestra las fechas del año pasado. |
| January | `6` | Muestra las fechas que están en enero, sin importar el año. |
| October | `7` | Muestra las fechas que están en octubre, sin importar el año. |
| November | `8` | Muestra las fechas que están en noviembre, sin importar el año. |
| December | `9` | Muestra las fechas que están en diciembre, sin importar el año. |
| February | `10` | Muestra las fechas que están en febrero, sin importar el año. |
| March | `11` | Muestra las fechas que están en marzo, sin importar el año. |
| April | `12` | Muestra las fechas que están en abril, sin importar el año. |
| May | `13` | Muestra las fechas que están en mayo, sin importar el año. |
| June | `14` | Muestra las fechas que están en junio, sin importar el año. |
| July | `15` | Muestra las fechas que están en julio, sin importar el año. |
| August | `16` | Muestra las fechas que están en agosto, sin importar el año. |
| September | `17` | Muestra las fechas que están en septiembre, sin importar el año. |
| NextMonth | `18` | Muestra las fechas del próximo mes. |
| NextQuarter | `19` | Muestra las fechas del próximo trimestre. |
| NextWeek | `20` | Muestra las fechas de la próxima semana. |
| NextYear | `21` | Muestra las fechas del próximo año. |
| None | `22` | Ninguno. |
| Quarter1 | `23` | Muestra las fechas que están en el 1.º trimestre, sin importar el año. |
| Quarter2 | `24` | Muestra las fechas que están en el 2.º trimestre, sin importar el año. |
| Quarter3 | `25` | Muestra las fechas que están en el 3.º trimestre, sin importar el año. |
| Quarter4 | `26` | Muestra las fechas que están en el 4.º trimestre, sin importar el año. |
| ThisMonth | `27` | Muestra las fechas de este mes. |
| ThisQuarter | `28` | Muestra las fechas de este trimestre. |
| ThisWeek | `29` | Muestra las fechas de esta semana. |
| ThisYear | `30` | Muestra las fechas de este año. |
| Today | `31` | Muestra las fechas de hoy. |
| Tomorrow | `32` | Muestra las fechas de mañana. |
| YearToDate | `33` | Muestra las fechas entre el comienzo del año y hoy, inclusive. |
| Yesterday | `34` | Muestra las fechas de ayer. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterTypeDemo
    {
        public static void DynamicFilterTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            // Aplicar filtro automático a la hoja de cálculo
            worksheet.AutoFilter.SetRange(0, 0, 5);

            // Aplicar un filtro dinámico para mostrar solo las fechas de marzo
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            // Guarda el libro de trabajo
            workbook.Save("DynamicFilterTypeExample.xlsx");
            workbook.Save("DynamicFilterTypeExample.pdf");

            // Genere la salida de los resultados
            Console.WriteLine("Dynamic filter applied to show only dates in March.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


