---
title: "GlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GlobalizationSettings. Obtient le séparateur pour les lignes dans les données de tableau dans la formule"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/rowseparatorofformulaarray/
---
## GlobalizationSettings.RowSeparatorOfFormulaArray property

Obtient le séparateur des lignes dans les données de tableau dans la formule.

```csharp
public virtual char RowSeparatorOfFormulaArray { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Cr\u00e9er un nouveau classeur avec des param\u00e8tres de mondialisation personnalis\u00e9s
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à l'instance des paramètres de mondialisation personnalisés
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            // Affichez la valeur actuelle de RowSeparatorOfFormulaArray
            Console.WriteLine("Current RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Créez une formule de tableau en utilisant le séparateur de ligne personnalisé
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=SUM({1,2|3,4})"; // Uses '|' as row separator

            // Calculez la formule pour démontrer une analyse correcte
            workbook.CalculateFormula();

            // Afficher les résultats
            Console.WriteLine("Array formula using custom separator: " + cell.Formula);
            Console.WriteLine("Calculated result: " + cell.Value);

            // Enregistrez le classeur
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }

    // Implémentation personnalisée de GlobalizationSettings qui surcharge le séparateur de ligne
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override char RowSeparatorOfFormulaArray => '|';
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


