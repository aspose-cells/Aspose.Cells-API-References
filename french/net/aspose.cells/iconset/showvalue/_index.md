---
title: "IconSet.ShowValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété IconSet. Obtenir ou définir le drapeau indiquant s'il faut afficher les valeurs des cellules auxquelles cet ensemble d'icônes est appliqué. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/iconset/showvalue/
---
## IconSet.ShowValue property

Obtenir ou définir le drapeau indiquant s'il faut afficher les valeurs des cellules auxquelles cet ensemble d'icônes est appliqué. La valeur par défaut est true.

```csharp
public bool ShowValue { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyShowValueDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);
            sheet.Cells["A5"].PutValue(50);

            // Ajouter une mise en forme conditionnelle d'ensemble d'icônes
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            int index = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[index];

            // Définir les propriétés du jeu d'icônes
            condition.IconSet.Type = IconSetType.TrafficLights31;
            condition.IconSet.ShowValue = false; // This hides cell values and shows only icons
            condition.IconSet.Reverse = false;

            // Définir la plage pour la mise en forme conditionnelle
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            formatConditions.AddArea(area);

            // Enregistrez le classeur
            workbook.Save("IconSetShowValueDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon set conditional formatting (ShowValue = false).");
        }
    }
}
```

### Voir aussi

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


