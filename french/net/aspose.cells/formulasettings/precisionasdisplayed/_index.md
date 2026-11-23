---
title: "FormulaSettings.PrecisionAsDisplayed"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaSettings. Indique si la précision du résultat calculé doit être définie telle qu'elle est affichée lors du calcul des formules"
type: docs
url: /fr/net/aspose.cells/formulasettings/precisionasdisplayed/
---
## FormulaSettings.PrecisionAsDisplayed property

Indique si la précision du résultat calculé doit être définie telle qu'elle est affichée lors du calcul des formules.

```csharp
public bool PrecisionAsDisplayed { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPrecisionAsDisplayedDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Définir PrecisionAsDisplayed sur true
            workbook.Settings.FormulaSettings.PrecisionAsDisplayed = true;
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Définir le format d'affichage de la cellule A1 pour afficher 2 décimales
            cells["A1"].PutValue(1.23456);
            Style style = cells["A1"].GetStyle();
            style.Number = 2; // Format: 0.00
            cells["A1"].SetStyle(style);
            
            // Définir la formule dans B1 qui fait référence à A1
            cells["B1"].Formula = "=A1";
            
            // Calculer les formules avec PrecisionAsDisplayed activé
            workbook.CalculateFormula();
            
            // Afficher les résultats
            Console.WriteLine("A1 Display Value: " + cells["A1"].StringValue); // Shows 1.23
            Console.WriteLine("B1 Calculated Value: " + cells["B1"].Value);   // Should be 1.23 due to PrecisionAsDisplayed
        }
    }
}
```

### Voir aussi

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


