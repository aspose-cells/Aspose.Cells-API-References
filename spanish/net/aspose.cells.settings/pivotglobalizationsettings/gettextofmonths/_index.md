---
title: "PivotGlobalizationSettings.GetTextOfMonths"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto local de meses"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/
---
## PivotGlobalizationSettings.GetTextOfMonths method

Obtiene el texto local de "Months".

```csharp
public virtual string GetTextOfMonths()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMonthsDemo
    {
        public static void Run()
        {
            // Cree configuraciones de globalización personalizadas
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // Demostrar GetTextOfMonths
            Console.WriteLine("Custom Months Text: " + customSettings.GetTextOfMonths());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfMonths()
        {
            // Devuelve texto localizado personalizado para "Months"
            return "Custom Months Label";
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


