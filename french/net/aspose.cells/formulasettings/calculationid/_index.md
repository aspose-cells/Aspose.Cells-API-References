---
title: "FormulaSettings.CalculationId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaSettings. Spécifie la version du moteur de calcul utilisé pour calculer les valeurs dans le classeur"
type: docs
url: /fr/net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

Spécifie la version du moteur de calcul utilisé pour calculer les valeurs dans le classeur.

```csharp
public string CalculationId { get; set; }
```

### Remarques

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Dans le cas de MS Excel, si la valeur de cette propriété est inférieure à l'identifiant du moteur de recalcul associé à l'application qui ouvre le fichier résultant, l'application recalculera les résultats de toutes les formules de ce classeur immédiatement après le chargement du fichier. Pour des raisons de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule du classeur automatiquement, quel que soit la valeur définie pour cette propriété.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationIdDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Définir une formule qui se comporte différemment selon CalculationId
            Cell cell = sheet.Cells["A1"];
            cell.Formula = "=AND(\"a\",true)";
            
            // Calculer sans CalculationId (comportement par défaut)
            wb.CalculateFormula();
            Console.WriteLine("Without CalculationId: " + cell.Value);
            
            // Définir CalculationId et recalculer
            wb.Settings.FormulaSettings.CalculationId = "181029";
            wb.CalculateFormula();
            Console.WriteLine("With CalculationId 181029: " + cell.BoolValue);
        }
    }
}
```

### Voir aussi

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


