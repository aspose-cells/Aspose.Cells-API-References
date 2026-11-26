---
title: "PivotGlobalizationSettings.GetTextOfMinutes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto local de minutos"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/
---
## PivotGlobalizationSettings.GetTextOfMinutes method

Obtiene el texto local de "Minutes".

```csharp
public virtual string GetTextOfMinutes()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMinutesDemo
    {
        public static void Run()
        {
            // Crear una instancia de PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demostrar el método GetTextOfMinutes
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());

            // Demostración adicional de métodos de tiempo relacionados para contexto
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


