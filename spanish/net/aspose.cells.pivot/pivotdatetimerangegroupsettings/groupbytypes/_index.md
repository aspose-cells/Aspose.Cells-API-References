---
title: "PivotDateTimeRangeGroupSettings.GroupByTypes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotDateTimeRangeGroupSettings. Obtiene los tipos de agrupación por fecha y hora"
type: docs
url: /es/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/
---
## PivotDateTimeRangeGroupSettings.GroupByTypes property

Obtiene los tipos de agrupación por fecha y hora.

```csharp
public PivotGroupByType[] GroupByTypes { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDateTimeRangeGroupSettingsPropertyGroupByTypesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con fechas
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Crear tabla dinámica
                int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Agregar campos a la tabla dinámica
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Agrupar por fecha con múltiples tipos de agrupación
                PivotField dateField = pivotTable.RowFields[0];
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 12, 31);
                PivotGroupByType[] groupTypes = new PivotGroupByType[]
                {
                    PivotGroupByType.Months,
                    PivotGroupByType.Quarters
                };
                dateField.GroupBy(startDate, endDate, groupTypes, 1, false);

                // Acceder a la configuración del grupo y demostrar la propiedad GroupByTypes
                PivotDateTimeRangeGroupSettings groupSettings =
                    (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

                // Mostrar el valor de la propiedad GroupByTypes
                Console.WriteLine("GroupByTypes values:");
                foreach (PivotGroupByType type in groupSettings.GroupByTypes)
                {
                    Console.WriteLine(type);
                }

                // Guardar el resultado
                workbook.Save("GroupByTypesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


