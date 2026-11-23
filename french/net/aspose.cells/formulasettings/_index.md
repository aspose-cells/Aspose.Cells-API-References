---
title: "Classe FormulaSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.FormulaSettings classe. Paramètres des formules et du calcul"
type: docs
url: /fr/net/aspose.cells/formulasettings/
---
## FormulaSettings class

Paramètres des formules et du calcul.

```csharp
public class FormulaSettings
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CalculateOnOpen](../../aspose.cells/formulasettings/calculateonopen/) { get; set; } | Indique si l'application doit effectuer un calcul complet lorsque le classeur est ouvert. |
| [CalculateOnSave](../../aspose.cells/formulasettings/calculateonsave/) { get; set; } | Indique s'il faut recalculer le classeur avant d'enregistrer le document, lorsqu'il est en mode de calcul manuel. |
| [CalculationId](../../aspose.cells/formulasettings/calculationid/) { get; set; } | Spécifie la version du moteur de calcul utilisé pour calculer les valeurs dans le classeur. |
| [CalculationMode](../../aspose.cells/formulasettings/calculationmode/) { get; set; } | Obtient ou définit le mode de calcul du classeur dans MS Excel. |
| [EnableCalculationChain](../../aspose.cells/formulasettings/enablecalculationchain/) { get; set; } | Indique s'il faut activer la chaîne de calcul pour les formules. La valeur par défaut est false. |
| [EnableIterativeCalculation](../../aspose.cells/formulasettings/enableiterativecalculation/) { get; set; } | Indique s'il faut activer le calcul itératif pour résoudre les références circulaires. |
| [ForceFullCalculation](../../aspose.cells/formulasettings/forcefullcalculation/) { get; set; } | Indique s'il calcule toutes les formules à chaque déclenchement d'un calcul. |
| [MaxChange](../../aspose.cells/formulasettings/maxchange/) { get; set; } | Le changement maximal pour résoudre une référence circulaire. |
| [MaxIteration](../../aspose.cells/formulasettings/maxiteration/) { get; set; } | Le nombre maximal d'itérations pour résoudre une référence circulaire. |
| [PrecisionAsDisplayed](../../aspose.cells/formulasettings/precisionasdisplayed/) { get; set; } | Indique si la précision du résultat calculé doit être définie telle qu'elle est affichée lors du calcul des formules. |
| [PreservePaddingSpaces](../../aspose.cells/formulasettings/preservepaddingspaces/) { get; set; } | Indique s'il faut conserver les espaces et les sauts de ligne insérés entre les jetons de formule lors de la récupération et de la définition des formules. La valeur par défaut est false. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaSettingsDemo
    {
        public static void FormulaSettingsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux paramètres de formule du classeur
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Définition des propriétés
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationMode = CalcModeType.Automatic;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Enregistrez le classeur
            workbook.Save("FormulaSettingsExample.xlsx");
            workbook.Save("FormulaSettingsExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


