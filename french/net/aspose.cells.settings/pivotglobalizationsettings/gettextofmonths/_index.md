---
title: "PivotGlobalizationSettings.GetTextOfMonths"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte local des Mois"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/
---
## PivotGlobalizationSettings.GetTextOfMonths method

Obtient le texte local de "Months".

```csharp
public virtual string GetTextOfMonths()
```

### Exemples

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
            // Créer des paramètres de mondialisation personnalisés
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // Démontrez la méthode GetTextOfMonths
            Console.WriteLine("Custom Months Text: " + customSettings.GetTextOfMonths());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfMonths()
        {
            // Retourne un texte localisé personnalisé pour "Months"
            return "Custom Months Label";
        }
    }
}
```

### Voir aussi

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


