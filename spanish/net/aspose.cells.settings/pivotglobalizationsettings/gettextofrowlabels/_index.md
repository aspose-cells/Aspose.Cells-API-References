---
title: "PivotGlobalizationSettings.GetTextOfRowLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto de la etiqueta Etiquetas de fila en la tabla dinámica."
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/
---
## PivotGlobalizationSettings.GetTextOfRowLabels method

Obtiene el texto de la etiqueta "Row Labels" en la tabla dinámica.

```csharp
public virtual string GetTextOfRowLabels()
```

### Valor de retorno

El texto de las etiquetas de fila

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B3"].PutValue(200);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crear y usar configuraciones de globalización
            PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
            
            // Demostrar GetTextOfRowLabels
            Console.WriteLine("Row Labels Text: " + settings.GetTextOfRowLabels());

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


