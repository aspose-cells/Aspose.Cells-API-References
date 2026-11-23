---
title: "SettableGlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SettableGlobalizationSettings. Obtient le séparateur des lignes dans les données de tableau dans la formule"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/
---
## SettableGlobalizationSettings.RowSeparatorOfFormulaArray property

Obtient le séparateur des lignes dans les données de tableau dans la formule.

```csharp
public override char RowSeparatorOfFormulaArray { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une instance de SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Afficher le séparateur de ligne par défaut pour les tableaux de formules
            Console.WriteLine("Default RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Définir un nouveau séparateur de ligne pour les tableaux de formules
            settings.SetRowSeparatorOfFormulaArray(';');

            // Appliquer les paramètres au classeur
            workbook.Settings.GlobalizationSettings = settings;

            // Créer une formule de tableau dans la feuille de calcul
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            worksheet.Cells["A2"].SetArrayFormula("=SUM(A1:C2)", 1, 1);

            // Calculer les formules
            workbook.CalculateFormula();

            // Enregistrez le classeur
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


