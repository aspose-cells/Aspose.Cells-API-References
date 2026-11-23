---
title: "GlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GlobalizationSettings. Obtient le séparateur des éléments dans les données de lignes de tableau en formule"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/columnseparatorofformulaarray/
---
## GlobalizationSettings.ColumnSeparatorOfFormulaArray property

Obtient le séparateur des éléments dans les données de ligne du tableau dans la formule.

```csharp
public virtual char ColumnSeparatorOfFormulaArray { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des paramètres de mondialisation personnalisés avec un séparateur de colonne remplacé
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Afficher la valeur actuelle du séparateur de colonne
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " +
                globalizationSettings.ColumnSeparatorOfFormulaArray);

            // Créer une formule de tableau en utilisant un séparateur personnalisé
            Cell cell = worksheet.Cells["A1"];
            cell.SetArrayFormula("=SUM({1;2;3;4})", 1, 1); // Uses custom ';' column separator

            // Vérifier le stockage de la formule (afficherait des points-virgules dans la chaîne de formule réelle)
            Console.WriteLine("Stored array formula: " + cell.Formula);

            // Enregistrer le classeur modifié
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ColumnSeparatorOfFormulaArray => ';';
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


