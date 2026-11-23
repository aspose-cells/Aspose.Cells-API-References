---
title: "LoadOptions.DefaultStyleSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Obtient les paramètres de style par défaut pour initialiser les styles du classeur"
type: docs
url: /fr/net/aspose.cells/loadoptions/defaultstylesettings/
---
## LoadOptions.DefaultStyleSettings property

Obtient les paramètres de style par défaut pour initialiser les styles du classeur

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir les options de chargement avec les paramètres de style par défaut
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
            
            // Créer une feuille de calcul et obtenir les cellules
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Définir des valeurs pour démontrer le style par défaut
            cells["A1"].PutValue("Default Style Applied");
            cells["A2"].PutValue("Should have bottom alignment");
            
            // Créer une cellule avec un style personnalisé (pour contraster avec le style par défaut)
            Cell customCell = cells["B1"];
            customCell.PutValue("Custom Style");
            Style customStyle = customCell.GetStyle();
            customStyle.VerticalAlignment = TextAlignmentType.Center;
            customCell.SetStyle(customStyle);
            
            // Enregistrez le classeur
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
            
            // Vérifier les styles
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("B1 Vertical Alignment: " + cells["B1"].GetStyle().VerticalAlignment);
        }
    }
}
```

### Voir aussi

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


