---
title: "FormatCondition.Top10"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. Obtient l'instance Top10 du formatage conditionnel. La règle d'instance par défaut met en surbrillance les cellules dont les valeurs se situent dans les 10 premières positions. Valide uniquement pour le type Top10"
type: docs
url: /fr/net/aspose.cells/formatcondition/top10/
---
## FormatCondition.Top10 property

Obtenez l'instance "Top10" de la mise en forme conditionnelle. La règle de l'instance par défaut met en surbrillance les cellules dont les valeurs se situent dans le top 10. Valide uniquement pour le type = Top10.

```csharp
public Top10 Top10 { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTop10Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            Top10 top10 = fc.Top10;
            top10.IsPercent = true;
            top10.IsBottom = true;
            top10.Rank = 10;

            workbook.Save("FormatConditionPropertyTop10Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Top10](../../top10/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


