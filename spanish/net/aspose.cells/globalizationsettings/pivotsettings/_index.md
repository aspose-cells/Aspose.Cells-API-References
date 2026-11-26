---
title: "GlobalizationSettings.PivotSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GlobalizationSettings. Obtiene o establece la configuración de globalización para la tabla dinámica"
type: docs
url: /es/net/aspose.cells/globalizationsettings/pivotsettings/
---
## GlobalizationSettings.PivotSettings property

Obtiene o establece la configuración de globalización para la tabla dinámica.

```csharp
public PivotGlobalizationSettings PivotSettings { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfTotal()
        {
            return "Custom Total";
        }

        public override string GetTextOfGrandTotal()
        {
            return "Custom Grand Total";
        }

        public override string GetTextOfDataFieldHeader()
        {
            return "DataCaption";
        }

        public override string GetTextOfProtectedName(string protectedName)
        {
            return protectedName + "2";
        }
    }

    public class GlobalizationSettingsPropertyPivotSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de ejemplo
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Orange");
            dataSheet.Cells["B3"].PutValue(2000);

            // Crear tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int index = pivotSheet.PivotTables.Add("A1", "A1:B3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Establecer configuraciones de globalización personalizadas para la tabla dinámica
            CustomPivotGlobalizationSettings pivotSettings = new CustomPivotGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = new GlobalizationSettings();
            workbook.Settings.GlobalizationSettings.PivotSettings = pivotSettings;

            // Actualizar la tabla dinámica para aplicar la configuración
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../../../aspose.cells.settings/pivotglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


