---
title: "GlobalizationSettings.GetGrandTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre del total general de la función"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getgrandtotalname/
---
## GlobalizationSettings.GetGrandTotalName method

Obtiene el nombre del total general de la función.

```csharp
public virtual string GetGrandTotalName(ConsolidationFunction functionType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionType | ConsolidationFunction | El tipo de función. |

### Valor de retorno

El nombre del total general de la función.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos de ejemplo para la tabla dinámica
            CreateSampleData(worksheet);

            // Instanciar configuraciones de globalización personalizadas
            var globalizationSettings = new CustomGlobalizationSettings();
            
            try
            {
                // Demostrar llamada directa al método
                string grandTotalName = globalizationSettings.GetGrandTotalName(ConsolidationFunction.Sum);
                Console.WriteLine($"Grand Total Name: {grandTotalName}");

                // Aplicar personalización a la configuración del libro de trabajo
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Crear tabla dinámica para demostrar el efecto
                CreatePivotTable(worksheet);

                Console.WriteLine("Method executed successfully. Check output file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("GrandTotalNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            var cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Value";
            cells["A2"].Value = "Electronics";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Furniture";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Electronics";
            cells["B4"].Value = 800;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // Crear tabla dinámica usando un rango de datos de muestra
            int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Configurar campos de la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.Function = ConsolidationFunction.Sum;

            // Actualizar la tabla para aplicar la configuración
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetGrandTotalName(ConsolidationFunction functionType)
        {
            // Implementación personalizada basada en la función de consolidación
            return functionType == ConsolidationFunction.Sum 
                ? "**[Sum Total]**" 
                : base.GetGrandTotalName(functionType);
        }
    }
}
```

### Ver también

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


