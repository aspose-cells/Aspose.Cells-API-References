---
title: "GlobalizationSettings.GetPivotTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de la etiqueta Total en la tabla dinámica. Necesita sobrescribir este método cuando la tabla dinámica contiene dos o más PivotFields en el área de datos"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getpivottotalname/
---
## GlobalizationSettings.GetPivotTotalName method

Obtiene el nombre de la etiqueta "Total" en la tabla dinámica. Necesita sobrescribir este método cuando la tabla dinámica contiene dos o más PivotFields en el área de datos.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotTotalName()
```

### Valor de retorno

El nombre de la etiqueta "Total"

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetPivotTotalNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellene datos de ejemplo
            worksheet.Cells["A1"].Value = "Region";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "North"; worksheet.Cells["B2"].Value = 1000; worksheet.Cells["C2"].Value = 50;
            worksheet.Cells["A3"].Value = "South"; worksheet.Cells["B3"].Value = 2000; worksheet.Cells["C3"].Value = 70;
            worksheet.Cells["A4"].Value = "West"; worksheet.Cells["B4"].Value = 3000; worksheet.Cells["C4"].Value = 110;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E5", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Quantity

            // Crear y configurar configuraciones de globalización
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Demostrar llamada directa al método
                Console.WriteLine("Custom Total Name: " + customSettings.GetPivotTotalName());

                // Procesar tabla dinámica
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Pivot table created with custom total name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("MethodGetPivotTotalNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetPivotTotalName()
        {
            return "Custom Total";
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


