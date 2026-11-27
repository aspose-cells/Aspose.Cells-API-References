---
title: "Klass FormatConditionCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FormatConditionCollection-klass. Representerar villkorlig formatering. FormatConditions kan innehålla upp till tre villkorliga format"
type: docs
url: /sv/net/aspose.cells/formatconditioncollection/
---
## FormatConditionCollection class

Representerar villkorsstyrd formatering. FormatConditions kan innehålla upp till tre villkorsformat.

```csharp
public class FormatConditionCollection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count/) { get; } | Hämtar antalet villkor. |
| [Item](../../aspose.cells/formatconditioncollection/item/) { get; } | Hämtar formateringsvillkoret efter index. |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount/) { get; } | Hämtar antalet villkorligt formaterade områden. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add/)(CellArea, FormatConditionType, OperatorType, string, string) | Lägger till ett formateringsvillkor och påverkad cellområde till FormatConditions. FormatConditions kan innehålla upp till tre villkorliga format. Referenser till andra blad är inte tillåtna i formlerna för villkorlig formatering. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea/)(CellArea) | Lägger till ett villkorligt formaterat cellområde. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition)(FormatConditionType) | Lägg till ett formatvillkor. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition_1)(FormatConditionType, OperatorType, string, string) | Lägger till ett formateringsvillkor. |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea/)(int) | Hämtar det villkorligt formaterade cellområdet efter index. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea_1)(int) | Tar bort det villkorligt formaterade cellområdet efter index. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea)(int, int, int, int) | Ta bort villkorlig formatering i området. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition/)(int) | Tar bort formateringsvillkoret efter index. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionDemo
    {
        public static void FormatConditionCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Hämta det första kalkylbladet
            Worksheet sheet = workbook.Worksheets[0];

            // Lägger till en tom villkorlig formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Ställer in området för den villkorliga formateringen
            CellArea ca = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);
            ca = new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 };
            fcs.AddArea(ca);

            // Lägger till villkor
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // Ställer in bakgrundsfärgen
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Red;

            // Sparar Excel-filen
            workbook.Save("FormatConditionCollectionExample.xlsx");
            workbook.Save("FormatConditionCollectionExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


