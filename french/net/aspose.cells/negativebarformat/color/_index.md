---
title: "NegativeBarFormat.Color"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété NegativeBarFormat. Obtient ou définit un objet FormatColor que vous pouvez utiliser pour spécifier la couleur de remplissage des barres de données négatives"
type: docs
url: /fr/net/aspose.cells/negativebarformat/color/
---
## NegativeBarFormat.Color property

Obtient ou définit un objet FormatColor que vous pouvez utiliser pour spécifier la couleur de remplissage des barres de données négatives.

```csharp
public Color Color { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyColorDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Créer une mise en forme conditionnelle
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Configurer les propriétés des barres de données
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Configurer le format des barres négatives
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Enregistrez le classeur
            workbook.Save("NegativeBarFormatColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("NegativeBarFormatPropertyColorDemo executed successfully.");
        }
    }
}
```

### Voir aussi

* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


