---
title: "SettableGlobalizationSettings.GetTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre total de una función específica"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/gettotalname/
---
## SettableGlobalizationSettings.GetTotalName method

Obtiene el nombre total de la función específica.

```csharp
public override string GetTotalName(ConsolidationFunction functionType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionType | ConsolidationFunction | El tipo de función. |

### Valor de retorno

El nombre total de la función.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una instancia de SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Llamar a GetTotalName con ConsolidationFunction.Sum
                string totalName = globalizationSettings.GetTotalName(ConsolidationFunction.Sum);
                
                // Mostrar el resultado
                Console.WriteLine($"Total name for Sum function: {totalName}");

                // Agregar datos para demostrar el efecto (aunque GetTotalName no modifica la hoja de cálculo)
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["B1"].PutValue("Total");
                worksheet.Cells["B4"].Formula = "=SUM(A2:A4)";
                
                // Calcular fórmulas
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTotalName method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("SettableGlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


