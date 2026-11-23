---
title: "DataBar.AxisColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataBar. Obtient la couleur de l'axe pour les cellules avec un format conditionnel sous forme de barres de données"
type: docs
url: /fr/net/aspose.cells/databar/axiscolor/
---
## DataBar.AxisColor property

Obtient la couleur de l'axe pour les cellules avec une mise en forme conditionnelle sous forme de barres de données.

```csharp
public Color AxisColor { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyAxisColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Définir des données d'exemple
            sheet.Cells["E3"].PutValue(10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-15);
            sheet.Cells["G4"].PutValue(-25);

            // Ajouter une mise en forme conditionnelle de barre de données
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Définir les propriétés de la barre de données
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;
            cond.DataBar.BarFillType = DataBarFillType.Solid;
            
            // Démontrer la propriété AxisColor
            cond.DataBar.AxisColor = Color.Red;
            cond.DataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // Définir le formatage des barres négatives
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Enregistrez le classeur
            workbook.Save("DataBarAxisColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


