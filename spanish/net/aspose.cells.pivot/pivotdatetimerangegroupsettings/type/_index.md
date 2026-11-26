---
title: "PivotDateTimeRangeGroupSettings.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotDateTimeRangeGroupSettings. Obtiene el tipo de grupo de fecha y hora de los datos"
type: docs
url: /es/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/type/
---
## PivotDateTimeRangeGroupSettings.Type property

Obtiene el tipo de grupo de fecha y hora.

```csharp
public override PivotFieldGroupType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
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

            // Agregar campos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Agrupar por fecha
            PivotField dateField = pivotTable.RowFields[0];
            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

            // Acceda a la configuración del grupo y demuestre la propiedad Type
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            Console.WriteLine("Group Type: " + groupSettings.Type);
            
            workbook.Save("PivotDateTimeGroupingDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


