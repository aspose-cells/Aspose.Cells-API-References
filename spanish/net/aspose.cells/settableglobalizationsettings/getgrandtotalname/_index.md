---
title: "SettableGlobalizationSettings.GetGrandTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre del total general de la función"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/getgrandtotalname/
---
## SettableGlobalizationSettings.GetGrandTotalName method

Obtiene el nombre del total general de la función.

```csharp
public override string GetGrandTotalName(ConsolidationFunction functionType)
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
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class SettableGlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Establezca nombres personalizados de total general para diferentes funciones de consolidación
            settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Sum Grand Total");
            settings.SetGrandTotalName(ConsolidationFunction.Average, "Custom Average Grand Total");
            
            // Aplicar la configuración al workbook
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Llame a GetGrandTotalName con diferentes funciones de consolidación
                string sumGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Sum);
                string avgGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Average);
                
                // Genere la salida de los resultados
                Console.WriteLine("Sum Grand Total Name: " + sumGrandTotalName);
                Console.WriteLine("Average Grand Total Name: " + avgGrandTotalName);

                // Crear una tabla dinámica para demostrar el efecto
                Cells cells = worksheet.Cells;
                cells["A1"].PutValue("Product");
                cells["B1"].PutValue("Sales");
                cells["A2"].PutValue("Apple");
                cells["B2"].PutValue(1000);
                cells["A3"].PutValue("Orange");
                cells["B3"].PutValue(2000);
                cells["A4"].PutValue("Banana");
                cells["B4"].PutValue(3000);

                PivotTableCollection pivotTables = worksheet.PivotTables;
                int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = pivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                
                // Forma correcta de agregar otro campo de datos con la función Average
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("SettableGlobalizationSettingsMethodGetGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


