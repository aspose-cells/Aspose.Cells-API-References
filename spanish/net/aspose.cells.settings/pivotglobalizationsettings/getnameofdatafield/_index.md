---
title: "PivotGlobalizationSettings.GetNameOfDataField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el nombre para mostrar del campo de datos de pivote. El formato predeterminado es Suma de Campo"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/
---
## PivotGlobalizationSettings.GetNameOfDataField method

Obtiene el nombre para mostrar del campo de datos de la tabla dinámica. El formato predeterminado es "Sum Of Field".

```csharp
public virtual string GetNameOfDataField(ConsolidationFunction function, string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| función | ConsolidationFunction | La función se usa para resumir valores del campo de pivote. |
| name | String | El nombre original del campo de pivote. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetNameOfDataFieldWithConsolidationFuStringDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una instancia de PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Definir parámetros para el método GetNameOfDataField
                ConsolidationFunction function = ConsolidationFunction.Sum;
                string fieldName = "Sales";

                // Llamar al método GetNameOfDataField
                string result = globalizationSettings.GetNameOfDataField(function, fieldName);

                // Mostrar el resultado
                Console.WriteLine($"Localized name for data field '{fieldName}' with function '{function}': {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNameOfDataField: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


