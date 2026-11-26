---
title: "PivotGlobalizationSettings.GetTextOfYears"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto local de Años."
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofyears/
---
## PivotGlobalizationSettings.GetTextOfYears method

Obtiene el texto local de "Years".

```csharp
public virtual string GetTextOfYears()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfYearsDemo
    {
        public static void Run()
        {
            // Cree configuraciones de globalización personalizadas
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // Demostrar el método GetTextOfYears
            Console.WriteLine("Custom Text of Years: " + customSettings.GetTextOfYears());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfYears()
        {
            // Devolver texto personalizado para la etiqueta "Años"
            return "Custom Years Label";
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


