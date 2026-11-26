---
title: "GlobalizationSettings.GetEmptyDataName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de la etiqueta en blanco en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getemptydataname/
---
## GlobalizationSettings.GetEmptyDataName method

Obtiene el nombre de la etiqueta "(blank)" en la tabla dinámica.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfEmptyData() method instead.")]
public virtual string GetEmptyDataName()
```

### Valor de retorno

El nombre de los datos vacíos

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetColumnLabelsOfPivotTable(). Esta propiedad será eliminada 12 meses después desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetEmptyDataNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra con celdas vacías
            object[,] data = new object[,]
            {
                {"Category", "Sales"},
                {"Electronics", 1500},
                {null, 2000}, // Empty category cell
                {"Furniture", 3000}
            };

            // Poblar la hoja de cálculo
            int rows = data.GetLength(0);
            int cols = data.GetLength(1);
            for (int i = 0; i < rows; i++)
            {
                for (int j = 0; j < cols; j++)
                {
                    worksheet.Cells[i, j].PutValue(data[i, j]);
                }
            }

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            // Corregido: Eliminar la asignación no válida del resultado de AddFieldToArea
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configurar configuraciones de globalización personalizadas
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Actualizar la tabla dinámica para aplicar la localización
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Demostrar llamada directa al método
                string emptyName = workbook.Settings.GlobalizationSettings.GetEmptyDataName();
                Console.WriteLine($"Custom empty data label: {emptyName}");

                workbook.Save("GlobalizationGetEmptyDataNameDemo.xlsx");
                Console.WriteLine("Demo executed successfully. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            [Obsolete]
            public override string GetEmptyDataName()
            {
                return "[[UNSPECIFIED]]"; // Custom empty data label
            }
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


