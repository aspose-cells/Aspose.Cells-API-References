---
title: "Clase PivotDateTimeRangeGroupSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotDateTimeRangeGroupSettings. Representa el campo agrupado por rango de fecha y hora"
type: docs
url: /es/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/
---
## PivotDateTimeRangeGroupSettings class

Representa el campo agrupado por rango de fecha y hora.

```csharp
public class PivotDateTimeRangeGroupSettings : PivotFieldGroupSettings
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [End](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/end/) { get; } | Obtiene la fecha y hora de finalización del grupo. |
| [GroupByTypes](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/) { get; } | Obtiene los tipos de agrupación por fecha y hora. |
| [Interval](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/) { get; } | Obtiene el interno del grupo. |
| [Start](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/start/) { get; } | Obtiene la fecha y hora de inicio del grupo. |
| override [Type](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/type/) { get; } | Obtiene el tipo de grupo de fecha y hora. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [IsGroupedBy](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/isgroupedby/)(PivotGroupByType) | Comprueba si el campo está agrupado por el tipo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotDateTimeRangeGroupSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar datos de muestra con fechas
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);

                // Crear tabla dinámica
                int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Agregar campos a la tabla dinámica
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Agrupar el campo de fecha por meses
                PivotField dateField = pivotTable.RowFields[0];
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 12, 31);
                dateField.GroupBy(startDate, endDate, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

                // Obtener la configuración del grupo
                PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

                // Mostrar propiedades de la configuración del grupo
                Console.WriteLine($"Group Type: {groupSettings.Type}");
                Console.WriteLine($"Start Date: {groupSettings.Start}");
                Console.WriteLine($"End Date: {groupSettings.End}");
                Console.WriteLine($"Interval: {groupSettings.Interval}");
                Console.WriteLine($"Group By Types: {string.Join(", ", groupSettings.GroupByTypes)}");

                // Comprobar si está agrupado por meses
                bool isGroupedByMonths = groupSettings.IsGroupedBy(PivotGroupByType.Months);
                Console.WriteLine($"Is grouped by months: {isGroupedByMonths}");

                // Guarda el libro de trabajo
                workbook.Save("PivotDateTimeRangeGroupSettingsDemo.xlsx");
                Console.WriteLine("PivotDateTimeRangeGroupSettings demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in PivotDateTimeRangeGroupSettings demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


