---
title: "PivotGlobalizationSettings.GetTextOfDays"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto local de Días"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofdays/
---
## PivotGlobalizationSettings.GetTextOfDays method

Obtiene el texto local de "Days".

```csharp
public virtual string GetTextOfDays()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfDaysDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B3"].PutValue(1500);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregue el campo de fecha al área de filas
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Crear configuraciones de globalización
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demuestre el método GetTextOfDays
            Console.WriteLine("Localized text for days: " + globalizationSettings.GetTextOfDays());

            // Guarda el libro de trabajo
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


