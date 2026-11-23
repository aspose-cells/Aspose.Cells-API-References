---
title: "DataBar.BarFillType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataBar. Obtient ou définit comment une barre de données est remplie de couleur"
type: docs
url: /fr/net/aspose.cells/databar/barfilltype/
---
## DataBar.BarFillType property

Obtient ou définit comment une barre de données est remplie de couleur.

```csharp
public DataBarFillType BarFillType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarFillTypeDemo
    {
        public static void Run()
        {
            // Instanciez un objet Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une mise en forme conditionnelle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Définir la plage du format conditionnel
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 5,
                StartColumn = 0,
                EndColumn = 5
            };
            fcs.AddArea(ca);

            // Ajouter une condition DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Configurer les propriétés DataBar
            DataBar dataBar = fc.DataBar;
            dataBar.BarFillType = DataBarFillType.Gradient; // Demonstrating BarFillType usage
            dataBar.Color = Color.Blue;

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(100);

            // Enregistrez le classeur
            workbook.Save("DataBarFillTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [DataBarFillType](../../databarfilltype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


