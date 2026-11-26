---
title: "GlobalizationSettings.GetColumnLabelsOfPivotTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de la etiqueta Column Labels en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getcolumnlabelsofpivottable/
---
## GlobalizationSettings.GetColumnLabelsOfPivotTable method

Obtiene el nombre de la etiqueta "Column Labels" en la tabla dinámica.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfColumnLabels() method instead.")]
public virtual string GetColumnLabelsOfPivotTable()
```

### Valor de retorno

El nombre de las etiquetas de columna

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetColumnLabelsOfPivotTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 10000;
            worksheet.Cells["A3"].Value = "Bike";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 8000;
            worksheet.Cells["A4"].Value = "Car";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 25000;

            // Crear una tabla dinámica y obtener una referencia
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C4", "E5");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Aplicar configuraciones de globalización personalizadas para sobrescribir las etiquetas de columna
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Actualizar y calcular la tabla dinámica para aplicar las configuraciones
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("GetColumnLabelsOfPivotTable method executed successfully. Check 'output.xlsx'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }

    // Implementación personalizada de GlobalizationSettings para sobrescribir las etiquetas de columna
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetColumnLabelsOfPivotTable()
        {
            // Devolver etiqueta personalizada para los encabezados de columna de la tabla dinámica
            return "Sales Regions";
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


