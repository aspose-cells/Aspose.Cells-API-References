---
title: "PivotGlobalizationSettings.GetTextOfSeconds"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto local de Seconds"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/
---
## PivotGlobalizationSettings.GetTextOfSeconds method

Obtiene el texto local de "Seconds"

```csharp
public virtual string GetTextOfSeconds()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfSecondsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue(100);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B2", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregue el campo de fecha al área de filas
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Crear configuraciones de globalización
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demostrar el método GetTextOfSeconds
            Console.WriteLine("Localized text for seconds: " + globalizationSettings.GetTextOfSeconds());

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


