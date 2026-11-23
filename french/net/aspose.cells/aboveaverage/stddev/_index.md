---
title: "AboveAverage.StdDev"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AboveAverage. Obtient ou définit le nombre d'écarts-types à inclure au-dessus ou en dessous de la moyenne dans la règle de mise en forme conditionnelle. La valeur d'entrée doit être comprise entre 0 et 3, incluant 0 et 3. Définir cette valeur à 0 signifie que stdDev n'est pas défini. La valeur par défaut est 0."
type: docs
url: /fr/net/aspose.cells/aboveaverage/stddev/
---
## AboveAverage.StdDev property

Obtenez ou définissez le nombre d'écarts‑type à inclure au‑dessus ou en dessous de la moyenne dans la règle de mise en forme conditionnelle. La valeur d'entrée doit être comprise entre 0 et 3 (inclure 0 et 3). Régler cette valeur à 0 signifie que stdDev n'est pas défini. La valeur par défaut est 0.

```csharp
public int StdDev { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AboveAveragePropertyStdDevDemo
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
            fc.Style.BackgroundColor = Color.Yellow;

            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.StdDev = 2;

            // Remplissez des données d'exemple
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;
            worksheet.Cells["A4"].Value = 40;
            worksheet.Cells["A5"].Value = 50;

            workbook.Save("AboveAverageStdDevDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AboveAverage](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


