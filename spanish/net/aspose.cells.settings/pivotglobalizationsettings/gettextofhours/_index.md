---
title: "PivotGlobalizationSettings.GetTextOfHours"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto local de Horas"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofhours/
---
## PivotGlobalizationSettings.GetTextOfHours method

Obtiene el texto local de "Hours".

```csharp
public virtual string GetTextOfHours()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfHoursDemo
    {
        public static void Run()
        {
            // Crear una instancia de PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demuestre el método GetTextOfHours
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());

            // Demostración adicional de métodos de tiempo relacionados
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


