---
title: "FormatCondition.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Hämtar och anger om den villkorliga formateringstypen"
type: docs
url: /sv/net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

Hämtar och anger om den villkorliga formattypen.

```csharp
public FormatConditionType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Skapa villkorlig formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Lägg till formatvillkor med uttryckstyp (korrigerade parametrar)
            int conditionIndex = fcs.AddCondition(FormatConditionType.Expression, OperatorType.None, "=A1>5", null);
            FormatCondition fc = fcs[conditionIndex];
            
            // Ange stil för villkoret
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Demonstrera användning av Type-egenskapen
            Console.WriteLine("Format Condition Type: " + fc.Type);
            
            // Spara arbetsboken
            workbook.Save("FormatConditionPropertyTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


