---
title: "FormulaSettings.CalculationMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaSettings. Obtient ou définit le mode de calcul du classeur dans MS Excel"
type: docs
url: /fr/net/aspose.cells/formulasettings/calculationmode/
---
## FormulaSettings.CalculationMode property

Obtient ou définit le mode de calcul du classeur dans MS Excel.

```csharp
public CalcModeType CalculationMode { get; set; }
```

### Remarques

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Pour des considérations de performance dans la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quel que soit le mode défini pour cette propriété. Si l'utilisateur doit calculer des formules, veuillez toujours appeler les méthodes sur différents objets selon les besoins : [`CalculateFormula`](../../workbook/calculateformula/), [`CalculateFormula`](../../worksheet/calculateformula/), [`Calculate`](../../cell/calculate/), ...etc.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationModeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir le mode de calcul sur AutomaticExceptTable
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.AutomaticExceptTable;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Modifier le mode de calcul en Manual
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // Réinitialiser au mode Automatic par défaut
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Automatic;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
        }
    }
}
```

### Voir aussi

* enum [CalcModeType](../../calcmodetype/)
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


