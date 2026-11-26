---
title: "PivotGlobalizationSettings.GetTextOfColumnLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto de la etiqueta Column Labels en la PivotTable"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofcolumnlabels/
---
## PivotGlobalizationSettings.GetTextOfColumnLabels method

Obtiene el texto de la etiqueta "Column Labels" en la tabla dinámica.

```csharp
public virtual string GetTextOfColumnLabels()
```

### Valor de retorno

El texto de las etiquetas de columna

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfColumnLabelsDemo
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
            worksheet.Cells["B3"].PutValue(800);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crear y usar configuraciones de globalización
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demostrar GetTextOfColumnLabels
            Console.WriteLine("Column Labels Text: " + globalizationSettings.GetTextOfColumnLabels());

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


