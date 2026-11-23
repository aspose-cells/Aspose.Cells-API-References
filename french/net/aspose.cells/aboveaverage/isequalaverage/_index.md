---
title: "AboveAverage.IsEqualAverage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AboveAverage. Obtient ou définit le drapeau indiquant si les critères aboveAverage et belowAverage sont inclusifs de la moyenne elle‑même ou exclusifs de cette valeur. true indique d’inclure la valeur moyenne dans les critères. La valeur par défaut est false."
type: docs
url: /fr/net/aspose.cells/aboveaverage/isequalaverage/
---
## AboveAverage.IsEqualAverage property

Obtenez ou définissez le drapeau indiquant si les critères 'aboveAverage' et 'belowAverage' sont inclusifs de la moyenne elle‑même, ou exclusifs de cette valeur. 'true' indique d’inclure la valeur moyenne dans les critères. La valeur par défaut est false.

```csharp
public bool IsEqualAverage { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyIsEqualAverageDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.LightBlue;

            // Démontrer la propriété IsEqualAverage
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false; // Cells equal to average won't be formatted

            // Remplissez des données d'exemple
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50; // Average is 30

            workbook.Save("AboveAverageIsEqualAverageDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


