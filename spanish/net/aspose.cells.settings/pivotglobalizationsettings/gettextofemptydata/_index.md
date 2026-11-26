---
title: "PivotGlobalizationSettings.GetTextOfEmptyData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto de la etiqueta en blanco en la PivotTable"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofemptydata/
---
## PivotGlobalizationSettings.GetTextOfEmptyData method

Obtiene el texto de la etiqueta "(blank)" en la tabla dinámica.

```csharp
public virtual string GetTextOfEmptyData()
```

### Valor de retorno

El texto de datos vacíos

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1500);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crear y usar PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demostrar el método GetTextOfEmptyData
            Console.WriteLine("Empty Data Text: " + globalizationSettings.GetTextOfEmptyData());

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


