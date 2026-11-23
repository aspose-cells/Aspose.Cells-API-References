---
title: "FormatCondition.TimePeriod"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FormatCondition. La période de temps applicable dans une règle de mise en forme conditionnelle basée sur une date. Valide uniquement pour le type timePeriod. La valeur par défaut est TimePeriodType.Today"
type: docs
url: /fr/net/aspose.cells/formatcondition/timeperiod/
---
## FormatCondition.TimePeriod property

La période de temps applicable dans une règle de mise en forme conditionnelle "date occurrin". Valide uniquement pour le type = timePeriod. La valeur par défaut est TimePeriodType.Today.

```csharp
public TimePeriodType TimePeriod { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTimePeriodDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des valeurs de date d'exemple pour démontrer le formatage par période de temps
            worksheet.Cells["A1"].PutValue(DateTime.Now);
            worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));

            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(area);

            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;
            fc.TimePeriod = TimePeriodType.Today;

            workbook.Save("TimePeriodDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


