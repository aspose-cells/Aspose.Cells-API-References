---
title: "FormulaSettings.CalculateOnSave"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormulaSettings. Indique s'il faut recalculer le classeur avant d'enregistrer le document en mode de calcul manuel"
type: docs
url: /fr/net/aspose.cells/formulasettings/calculateonsave/
---
## FormulaSettings.CalculateOnSave property

Indique s'il faut recalculer le classeur avant d'enregistrer le document, lorsqu'il est en mode de calcul manuel.

```csharp
public bool CalculateOnSave { get; set; }
```

### Remarques

Cette propriété ne sert qu'à enregistrer les paramètres dans le fichier de feuille de calcul résultant afin que d'autres applications (comme MS Excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant. Pour des raisons de performance pour la plupart des applications des utilisateurs, nous ne calculons aucune formule du classeur automatiquement, quel que soit la valeur définie pour cette propriété.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnSaveDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la feuille de calcul et ajouter des données
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Désactiver CalculateOnSave (false par défaut)
            workbook.Settings.FormulaSettings.CalculateOnSave = false;
            
            // Enregistrer sans calculer les formules
            workbook.Save("output_without_calculation.xlsx");

            // Activer CalculateOnSave
            workbook.Settings.FormulaSettings.CalculateOnSave = true;
            
            // Enregistrer avec le calcul des formules
            workbook.Save("output_with_calculation.xlsx");
        }
    }
}
```

### Voir aussi

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


