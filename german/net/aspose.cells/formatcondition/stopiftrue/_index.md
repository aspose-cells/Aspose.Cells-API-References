---
title: "FormatCondition.StopIfTrue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Wenn diese Regel wahr ist, dürfen keine Regeln mit niedrigerer Priorität über diese Regel angewendet werden. Gilt nur für Excel 2007"
type: docs
url: /de/net/aspose.cells/formatcondition/stopiftrue/
---
## FormatCondition.StopIfTrue property

True, es dürfen keine Regeln mit niedrigerer Priorität über diese Regel angewendet werden, wenn diese Regel zu true evaluiert. Gilt nur für Excel 2007;

```csharp
public bool StopIfTrue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStopIfTrueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Fügen Sie eine Bedingung hinzu und setzen Sie StopIfTrue
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            FormatCondition condition = fcs[conditionIndex];
            condition.StopIfTrue = true;
            
            // Fügen Sie eine weitere Bedingung hinzu, die normalerweise die erste überschreiben würde
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "25", "");
            FormatCondition condition2 = fcs[conditionIndex2];
            condition2.StopIfTrue = false;

            // Speichere die Arbeitsmappe
            workbook.Save("StopIfTrueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


