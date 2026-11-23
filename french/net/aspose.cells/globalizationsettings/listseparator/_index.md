---
title: "GlobalizationSettings.ListSeparator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GlobalizationSettings. Obtient le séparateur pour les paramètres de liste de la fonction ...etc"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/listseparator/
---
## GlobalizationSettings.ListSeparator property

Obtient le séparateur pour les listes, les paramètres de fonction, ...etc.

```csharp
public virtual char ListSeparator { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Cr\u00e9er un nouveau classeur avec des param\u00e8tres de mondialisation personnalis\u00e9s
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            Worksheet worksheet = workbook.Worksheets[0];
            
            // Affichez la valeur actuelle de ListSeparator provenant de nos paramètres personnalisés
            Console.WriteLine("Current ListSeparator value: " + workbook.Settings.GlobalizationSettings.ListSeparator);

            // Créez une formule en utilisant le séparateur de liste personnalisé
            worksheet.Cells["A1"].Formula = "=CONCATENATE(\"Hello\"; \" World\")";
            worksheet.Cells["A2"].Formula = "=SUM(1;2;3)";

            // Calculez les formules avec le séparateur personnalisé
            workbook.CalculateFormula();

            // Afficher les résultats du calcul
            Console.WriteLine("Concatenation result: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Sum result: " + worksheet.Cells["A2"].Value);

            // Enregistrez avec des formules en utilisant le séparateur de liste personnalisé
            workbook.Save("ListSeparatorDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ListSeparator => ';';
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


