---
title: "NegativeBarFormat.ColorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété NegativeBarFormat. Obtient ou définit s'il faut utiliser la même couleur de remplissage que les barres de données positives"
type: docs
url: /fr/net/aspose.cells/negativebarformat/colortype/
---
## NegativeBarFormat.ColorType property

Obtient ou définit s'il faut utiliser la même couleur de remplissage que les barres de données positives.

```csharp
public DataBarNegativeColorType ColorType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-15);
            sheet.Cells["F4"].PutValue(25);
            sheet.Cells["G3"].PutValue(-5);
            sheet.Cells["G4"].PutValue(15);

            // Créer une plage de mise en forme conditionnelle
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 3;
            area.EndColumn = 6;

            // Ajouter une mise en forme conditionnelle de barre de données
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(area);
            
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Définir les propriétés de la barre de données
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            
            // Configurer le format de la barre négative
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Enregistrez le classeur
            workbook.Save("NegativeBarFormatDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Demo completed. File saved with negative bar formatting.");
        }
    }
}
```

### Voir aussi

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


