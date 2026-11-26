---
title: "Enumeración PivotGroupByType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Pivot.PivotGroupByType. Representa el tipo de agrupación."
type: docs
url: /es/net/aspose.cells.pivot/pivotgroupbytype/
---
## PivotGroupByType enumeration

Representa el tipo de agrupación.

```csharp
[Flags]
public enum PivotGroupByType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| RangeOfValues | `1` | Agrupar por números. |
| Numbers | `1` | Agrupar por números. |
| Seconds | `2` | Presenta el tipo de agrupación por segundos. |
| Minutes | `4` | Presenta el tipo de agrupación por minutos. |
| Hours | `8` | Presenta el tipo de agrupación por horas. |
| Days | `10` | Presenta el tipo de agrupación por días. |
| Months | `20` | Presenta el tipo de agrupación por meses. |
| Quarters | `40` | Presenta el tipo de agrupación por trimestres. |
| Years | `80` | Presenta el tipo de agrupación por años. |
| DateTimes | `FE` | Presenta todos los tipos de agrupación de fechas y horas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGroupByTypeDemo
    {
        public static void PivotGroupByTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14;//m/d/yyy
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].SetStyle(style);

            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].SetStyle(style);

            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A4"].SetStyle(style);

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value field

            //TODO
            PivotField dateField = pivotTable.RowFields[0];

            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // Acceder a la configuración del grupo
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

            // Exportar la configuración del grupo
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Start Date: " + groupSettings.Start);
            Console.WriteLine("End Date: " + groupSettings.End);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // Guarda el libro de trabajo
            workbook.Save("PivotGroupByTypeExample.xlsx");
            
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


