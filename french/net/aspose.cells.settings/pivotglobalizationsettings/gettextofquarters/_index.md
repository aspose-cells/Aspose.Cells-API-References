---
title: "PivotGlobalizationSettings.GetTextOfQuarters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte local de Quarters"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/
---
## PivotGlobalizationSettings.GetTextOfQuarters method

Obtenez le texte local de "Quarters".

```csharp
public virtual string GetTextOfQuarters()
```

### Exemples

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
            // Créez une instance des paramètres de mondialisation
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Démontrer la méthode GetTextOfQuarters
            Console.WriteLine("Quarter labels: " + globalizationSettings.GetTextOfQuarters());
            
            // Afficher d'autres libellés de périodes temporelles associés pour le contexte
            Console.WriteLine("Year labels: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Month labels: " + globalizationSettings.GetTextOfMonths());
        }
    }
}
```

### Voir aussi

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


