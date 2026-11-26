---
title: "PivotGlobalizationSettings.GetTextOfAll"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto de la etiqueta Todo en la tabla dinámica."
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofall/
---
## PivotGlobalizationSettings.GetTextOfAll method

Obtiene el texto de la etiqueta "(All)" en la tabla dinámica.

```csharp
public virtual string GetTextOfAll()
```

### Valor de retorno

El texto de la etiqueta "(All)"

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfAllDemo
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
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crear y usar configuraciones de globalización
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demostrar el método GetTextOfAll
            Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());

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


