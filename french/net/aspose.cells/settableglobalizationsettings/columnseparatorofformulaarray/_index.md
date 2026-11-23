---
title: "SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SettableGlobalizationSettings. Obtient le séparateur des éléments dans les données de lignes de tableaux dans la formule"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/
---
## SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property

Obtient le séparateur des éléments dans les données de ligne du tableau dans la formule.

```csharp
public override char ColumnSeparatorOfFormulaArray { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une instance de SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Afficher la valeur actuelle de ColumnSeparatorOfFormulaArray
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " + settings.ColumnSeparatorOfFormulaArray);

            // Définir une nouvelle valeur pour ColumnSeparatorOfFormulaArray
            settings.SetColumnSeparatorOfFormulaArray(';');

            // Appliquer les paramètres au classeur
            workbook.Settings.GlobalizationSettings = settings;

            // Créer une formule de tableau avec le séparateur personnalisé en utilisant SetArrayFormula
            worksheet.Cells["A1"].SetArrayFormula("SUM({1,2,3;4,5,6})", 1, 1);
            worksheet.Cells["A2"].Formula = "=SUM(A1)";

            // Calculer les formules
            workbook.CalculateFormula();

            // Afficher le résultat
            Console.WriteLine("Result of array formula calculation: " + worksheet.Cells["A2"].Value);

            // Enregistrez le classeur
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


