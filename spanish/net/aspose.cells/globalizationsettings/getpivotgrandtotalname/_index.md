---
title: "GlobalizationSettings.GetPivotGrandTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de la etiqueta Grand Total en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getpivotgrandtotalname/
---
## GlobalizationSettings.GetPivotGrandTotalName method

Obtiene el nombre de la etiqueta "Grand Total" en la tabla dinámica.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfGrandTotal() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetPivotGrandTotalName()
```

### Valor de retorno

El nombre de la etiqueta "Grand Total"

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetPivotGrandTotalNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer configuraciones de globalización personalizadas
            var settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Poblar datos de ejemplo para la tabla dinámica
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Q1";
            cells["C1"].Value = "Q2";
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = 1500;
            cells["C2"].Value = 2200;
            cells["A3"].Value = "Clothing";
            cells["B3"].Value = 900;
            cells["C3"].Value = 1300;

            // Crear tabla dinámica con múltiples campos de datos
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C3", "E4");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Q1
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Q2

            // Actualizar y calcular la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            try
            {
                // Demostrar la llamada a GetPivotGrandTotalName
                string grandTotalName = settings.GetPivotGrandTotalName();
                Console.WriteLine($"Custom Grand Total Name: {grandTotalName}");

                // Guardar el libro de trabajo modificado
                workbook.Save("GlobalizationSettingsMethodGetPivotGrandTotalNameDemo.xlsx");
                Console.WriteLine("Spreadsheet saved. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetPivotGrandTotalName()
            {
                return "[Custom Grand Total]";
            }
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


