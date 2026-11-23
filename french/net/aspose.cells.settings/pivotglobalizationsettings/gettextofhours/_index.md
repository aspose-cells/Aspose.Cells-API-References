---
title: "PivotGlobalizationSettings.GetTextOfHours"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte local de Hours"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofhours/
---
## PivotGlobalizationSettings.GetTextOfHours method

Obtient le texte local de "Hours".

```csharp
public virtual string GetTextOfHours()
```

### Exemples

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
            // Créer une instance de PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Démontrez la méthode GetTextOfHours
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());

            // Démonstration supplémentaire des méthodes temporelles associées
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### Voir aussi

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


