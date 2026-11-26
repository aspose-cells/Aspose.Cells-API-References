---
title: "PivotGlobalizationSettings.GetTextOfTotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto de la etiqueta Total en la PivotTable. Necesita sobrescribir este método cuando la PivotTable contiene dos o más PivotFields en el área de datos"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/
---
## PivotGlobalizationSettings.GetTextOfTotal method

Obtiene el texto de la etiqueta "Total" en la tabla dinámica. Necesita sobrescribir este método cuando la tabla dinámica contiene dos o más PivotFields en el área de datos.

```csharp
public virtual string GetTextOfTotal()
```

### Valor de retorno

El texto de la etiqueta "Total"

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crear y usar configuraciones de globalización
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demostrar el método GetTextOfTotal
            Console.WriteLine("Total label text: " + globalizationSettings.GetTextOfTotal());

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


