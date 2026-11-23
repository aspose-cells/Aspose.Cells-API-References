---
title: "SettableGlobalizationSettings.ListSeparator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SettableGlobalizationSettings. Obtient le séparateur des paramètres de liste de la fonction ...etc"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/listseparator/
---
## SettableGlobalizationSettings.ListSeparator property

Obtient le séparateur pour les listes, les paramètres de fonction, ...etc.

```csharp
public override char ListSeparator { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez une instance de SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Afficher la valeur actuelle de ListSeparator (la valeur par défaut est la virgule dans la plupart des paramètres régionaux)
            Console.WriteLine("Current ListSeparator value: " + settings.ListSeparator);
            
            // Définir une nouvelle valeur pour ListSeparator (par ex., point-virgule)
            settings.SetListSeparator(';');
            
            // Appliquer les paramètres au classeur
            workbook.Settings.GlobalizationSettings = settings;
            
            // Démontrer l'effet de ListSeparator lors de l'analyse des formules
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue("Data");
            
            // Créer une formule qui utilise le séparateur de liste
            worksheet.Cells["A3"].Formula = "=CONCATENATE(A1,A2)";
            
            // La formule utilisera le séparateur de liste personnalisé lors de l'analyse
            Console.WriteLine("Formula with custom separator: " + worksheet.Cells["A3"].Formula);
            
            // Enregistrez le classeur
            workbook.Save("PropertyListSeparatorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


