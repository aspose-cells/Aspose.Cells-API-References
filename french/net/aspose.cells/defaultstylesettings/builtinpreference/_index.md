---
title: "DefaultStyleSettings.BuiltInPreference"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "DefaultStyleSettings propriété. Indique si la propriété du format numérique est préférable lorsque le style définit à la fois un nombre intégré et un modèle personnalisé. La valeur par défaut est false, ce qui signifie que, par défaut, le modèle personnalisé sera utilisé pour formater les valeurs tant qu'il n'est pas vide pour un style."
type: docs
url: /fr/net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

Indique si la propriété de format numérique est préférable lorsque le style définit à la fois un nombre intégré et un modèle personnalisé. La valeur par défaut est false, ce qui signifie que, par défaut, le modèle personnalisé sera utilisé pour formater les valeurs tant qu'il n'est pas vide pour un style.

```csharp
public bool BuiltInPreference { get; set; }
```

### Remarques

Lors du chargement d'un classeur à partir d'un fichier modèle existant, il se peut que le nombre intégré et le modèle personnalisé soient tous deux définis pour un style. Cette propriété détermine si nous devons utiliser le nombre intégré ou le modèle personnalisé lors du formatage des valeurs avec le style.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyBuiltInPreferenceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres de style par défaut
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Démontrer la propriété BuiltInPreference
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12;

            // Appliquer à la feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Enregistrez le classeur
            workbook.Save("BuiltInPreferenceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


