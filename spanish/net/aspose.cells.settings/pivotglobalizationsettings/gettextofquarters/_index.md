---
title: "PivotGlobalizationSettings.GetTextOfQuarters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto local de Quarters"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/
---
## PivotGlobalizationSettings.GetTextOfQuarters method

Obtén el texto local de "Quarters".

```csharp
public virtual string GetTextOfQuarters()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfQuartersDemo
    {
        public static void Run()
        {
            // Cree una instancia de configuración de globalización
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demostrar el método GetTextOfQuarters
            Console.WriteLine("Quarter labels: " + globalizationSettings.GetTextOfQuarters());
            
            // Mostrar otras etiquetas de períodos de tiempo relacionados para el contexto
            Console.WriteLine("Year labels: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Month labels: " + globalizationSettings.GetTextOfMonths());
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


