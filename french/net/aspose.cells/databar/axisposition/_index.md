---
title: "DataBar.AxisPosition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataBar. Obtient ou définit la position de l'axe des DataBars spécifié par une règle de mise en forme conditionnelle."
type: docs
url: /fr/net/aspose.cells/databar/axisposition/
---
## DataBar.AxisPosition property

Obtient ou définit la position de l'axe des barres de données spécifié par une règle de mise en forme conditionnelle.

```csharp
public DataBarAxisPosition AxisPosition { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyAxisPositionDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
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
            
            // Configurer les propriétés du DataBar
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;
            
            // Définir la position de l'axe (démo principale)
            cond.DataBar.AxisPosition = DataBarAxisPosition.Automatic;
            cond.DataBar.AxisColor = Color.Red;

            // Enregistrez le classeur
            workbook.Save("DataBarAxisPositionDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar with AxisPosition demo created successfully.");
        }
    }
}
```

### Voir aussi

* enum [DataBarAxisPosition](../../databaraxisposition/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


