---
title: "Classe DefaultStyleSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DefaultStyleSettings. Paramètres pour les valeurs par défaut des propriétés de style des classeurs"
type: docs
url: /fr/net/aspose.cells/defaultstylesettings/
---
## DefaultStyleSettings class

Paramètres pour les valeurs par défaut des propriétés de style du classeur.

```csharp
public class DefaultStyleSettings
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BuiltInPreference](../../aspose.cells/defaultstylesettings/builtinpreference/) { get; set; } | Indique si la propriété de format numérique est préférable lorsque le style définit à la fois un nombre intégré et un modèle personnalisé. La valeur par défaut est false, ce qui signifie que, par défaut, le modèle personnalisé sera utilisé pour formater les valeurs tant qu'il n'est pas vide pour un style. |
| [FontName](../../aspose.cells/defaultstylesettings/fontname/) { get; set; } | Obtient/Définit le nom de police par défaut pour le classeur |
| [FontSize](../../aspose.cells/defaultstylesettings/fontsize/) { get; set; } | Obtient/Définit la taille de police standard par défaut pour le classeur. |
| [HorizontalAlignment](../../aspose.cells/defaultstylesettings/horizontalalignment/) { get; set; } | Obtient/Définit la valeur par défaut pour l'alignement horizontal |
| [VerticalAlignment](../../aspose.cells/defaultstylesettings/verticalalignment/) { get; set; } | Obtient/Définit la valeur par défaut pour l'alignement vertical |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultStyleSettingsDemo
    {
        public static void DefaultStyleSettingsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux paramètres de style par défaut du classeur
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Définition des propriétés
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12.0;
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
            defaultStyleSettings.VerticalAlignment = TextAlignmentType.Center;

            // Appliquez les paramètres de style par défaut à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            // Enregistrez le classeur
            workbook.Save("DefaultStyleSettingsExample.xlsx");
            workbook.Save("DefaultStyleSettingsExample.pdf");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


