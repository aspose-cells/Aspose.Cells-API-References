---
title: "PivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto para el nombre protegido especificado"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/
---
## PivotGlobalizationSettings.GetTextOfProtectedName method

Obtiene el texto para el nombre protegido especificado.

```csharp
public virtual string GetTextOfProtectedName(string protectedName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| protectedName | String | El nombre protegido en la PivotTable. |

### Valor de retorno

Los nombres protegidos locales de la PivotTable.

### Observaciones

En Ms Excel, algunos nombres no pueden usarse como nombre de PivotFields en la PivotTable. Son diferentes según la región; el usuario puede especificarlos explícitamente de acuerdo con la región utilizada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectedNameWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una instancia de PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Definir un nombre protegido para obtener su texto
                string protectedName = "SensitiveData";

                // Llamar al método GetTextOfProtectedName
                string result = globalizationSettings.GetTextOfProtectedName(protectedName);

                // Mostrar el resultado
                Console.WriteLine($"Text for protected name \"{protectedName}\": {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


