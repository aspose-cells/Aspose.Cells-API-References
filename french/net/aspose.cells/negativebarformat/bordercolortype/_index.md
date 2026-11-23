---
title: "NegativeBarFormat.BorderColorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété NegativeBarFormat. Indique s'il faut utiliser la même couleur de bordure que les barres de données positives"
type: docs
url: /fr/net/aspose.cells/negativebarformat/bordercolortype/
---
## NegativeBarFormat.BorderColorType property

Indique s'il faut utiliser la même couleur de bordure que les barres de données positives.

```csharp
public DataBarNegativeColorType BorderColorType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyBorderColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Ajouter une mise en forme conditionnelle de barre de données
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Configurer la barre de données
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Définir la bordure de la barre de données
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            // Définir le format de la barre négative
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            
            // Démontrer la propriété BorderColorType
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Enregistrez le classeur
            workbook.Save("NegativeBarFormatBorderColorTypeDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Demo completed. File saved.");
        }
    }
}
```

### Voir aussi

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


