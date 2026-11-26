---
title: "SettableGlobalizationSettings.GetLocalFunctionName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre de función dependiente de la configuración regional según el nombre de función estándar proporcionado"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/getlocalfunctionname/
---
## SettableGlobalizationSettings.GetLocalFunctionName method

Obtiene el nombre de la función dependiente de la configuración regional según el nombre estándar de la función proporcionado.

```csharp
public override string GetLocalFunctionName(string standardName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| standardName | String | Nombre de función estándar (configuración regional en-US). |

### Valor de retorno

Nombre de función dependiente de la configuración regional. La configuración regional fue especificada por el Workbook para el cual se utiliza esta configuración.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Establecer un nombre de función local personalizado para "SUM"
            settings.SetLocalFunctionName("SUM", "SOMME", true);

            // Aplicar la configuración al workbook
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Llamar a GetLocalFunctionName para obtener el nombre localizado
                string localName = settings.GetLocalFunctionName("SUM");
                
                // Mostrar el resultado
                Console.WriteLine($"Localized function name for 'SUM': {localName}");

                // Usar la función localizada en una celda
                worksheet.Cells["A1"].Formula = "=SOMME(B1:B5)";
                worksheet.Cells["B1"].PutValue(1);
                worksheet.Cells["B2"].PutValue(2);
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["B4"].PutValue(4);
                worksheet.Cells["B5"].PutValue(5);

                // Calcular fórmulas
                workbook.CalculateFormula();

                // Mostrar el resultado
                Console.WriteLine($"Calculation result with localized function: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalFunctionName method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("MethodGetLocalFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


