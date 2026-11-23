---
title: "DataBar.ShowValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataBar. Obtenir ou définir le drapeau indiquant s'il faut afficher les valeurs des cellules auxquelles ce DataBar est appliqué. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/databar/showvalue/
---
## DataBar.ShowValue property

Obtenir ou définir le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles ce DataBar est appliqué. La valeur par défaut est true.

```csharp
public bool ShowValue { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyShowValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Ajouter une mise en forme conditionnelle de barre de données
            int idx = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Ajouter une condition de DataBar
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            
            // Définir les propriétés de la barre de données
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.DataBar.Color = Color.Green;
            
            // Démontrer la propriété ShowValue
            fc.DataBar.ShowValue = true; // Show cell values along with data bars
            
            // Enregistrez le classeur
            workbook.Save("DataBarShowValueDemo.xlsx");
            
            Console.WriteLine("DataBar ShowValue demo completed. Output file: DataBarShowValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


