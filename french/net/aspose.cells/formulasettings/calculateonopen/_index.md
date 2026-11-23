---
title: "FormulaSettings.CalculateOnOpen"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaSettings. Indique si l'application doit effectuer un calcul complet lors de l'ouverture du classeur"
type: docs
url: /fr/net/aspose.cells/formulasettings/calculateonopen/
---
## FormulaSettings.CalculateOnOpen property

Indique si l'application doit effectuer un calcul complet lorsque le classeur est ouvert.

```csharp
public bool CalculateOnOpen { get; set; }
```

### Remarques

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement du fichier résultant. Pour des raisons de performances pour la plupart des applications des utilisateurs, nous ne calculons aucune formule dans le classeur automatiquement, quel que soit la valeur définie pour cette propriété.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnOpenDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la formule dans la cellule A1 qui fait référence à B1
            worksheet.Cells["A1"].Formula = "=B1";
            
            // Définir la valeur dans la cellule B1
            worksheet.Cells["B1"].PutValue(10);
            
            // Désactiver le calcul automatique des formules à l'ouverture
            workbook.Settings.FormulaSettings.CalculateOnOpen = false;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Rouvrir le classeur enregistré
            Workbook reopenedWorkbook = new Workbook("output.xlsx");
            
            // Vérifier que la formule n'a pas été calculée à l'ouverture
            Console.WriteLine("A1 value (should be 0 before calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
            
            // Calculer les formules manuellement
            reopenedWorkbook.CalculateFormula();
            
            // Vérifier que la formule a été calculée
            Console.WriteLine("A1 value (should be 10 after calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
        }
    }
}
```

### Voir aussi

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


