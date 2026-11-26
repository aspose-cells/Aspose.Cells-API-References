---
title: "GlobalizationSettings.GetRowLabelsNameOfPivotTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de la etiqueta Row Labels en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getrowlabelsnameofpivottable/
---
## GlobalizationSettings.GetRowLabelsNameOfPivotTable method

Obtiene el nombre de la etiqueta "Row Labels" en la tabla dinámica.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfRowLabels() method instead.")]
public virtual string GetRowLabelsNameOfPivotTable()
```

### Valor de retorno

El nombre de las etiquetas de fila

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetRowLabelsNameOfPivotTable()
        {
            return "Custom Row Labels";
        }
    }

    public class GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["A2"].PutValue("Bikes");
            cells["A3"].PutValue("Cars");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(1000);
            cells["B3"].PutValue(2500);

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B3", "E3", "SalesPivot");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field

            // Aplicar configuraciones de globalización personalizadas
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                Console.WriteLine("Pivot table created with custom row labels name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowLabelsNameOfPivotTable: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetRowLabelsNameOfPivotTableDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


