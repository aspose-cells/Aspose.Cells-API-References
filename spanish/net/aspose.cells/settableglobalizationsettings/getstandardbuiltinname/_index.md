---
title: "SettableGlobalizationSettings.GetStandardBuiltInName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el texto estándar del nombre incorporado según el texto dependiente de la configuración regional proporcionado"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/getstandardbuiltinname/
---
## SettableGlobalizationSettings.GetStandardBuiltInName method

Obtiene el texto estándar del Nombre incorporado según el texto dependiente de la configuración regional proporcionado.

```csharp
public override string GetStandardBuiltInName(string localName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| localName | String | Texto dependiente de la configuración regional del nombre incorporado. La configuración regional fue especificada por el Libro de trabajo para el cual se utilizan estos ajustes. |

### Valor de retorno

Texto estándar (configuración regional en-US).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una instancia de SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            // Establecer un nombre incorporado local para demostración
            globalizationSettings.SetLocalBuiltInName("SUM", "LocalSumName", true);

            try
            {
                // Llamar al método GetStandardBuiltInName con un nombre local
                string standardName = globalizationSettings.GetStandardBuiltInName("LocalSumName");
                
                // Mostrar el resultado
                Console.WriteLine($"Standard name for 'LocalSumName' is: {standardName}");

                // Aplicar el resultado a una celda
                worksheet.Cells["A1"].Formula = "=" + standardName + "(1,2,3)";
                workbook.CalculateFormula();

                // Mostrar el resultado calculado
                Console.WriteLine($"Result of formula in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


