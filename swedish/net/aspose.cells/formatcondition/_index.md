---
title: "Klass FormatCondition"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FormatCondition-klass. Representerar villkorligt formateringsvillkor"
type: docs
url: /sv/net/aspose.cells/formatcondition/
---
## FormatCondition class

Representerar villkoret för villkorsstyrd formatering.

```csharp
public class FormatCondition
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage/) { get; } | Hämta den villkorliga formateringens "AboveAverage"-instans. Standardinstansens regel markerar celler som ligger över genomsnittet för alla värden i intervallet. Giltig endast för typ = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale/) { get; } | Hämta den villkorliga formateringens "ColorScale"-instans. Standardinstansen är en "grön-gul-röd" 3ColorScale. Giltig endast för typ = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar/) { get; } | Hämta den villkorliga formateringens "DataBar"-instans. Standardinstansens färg är blå. Giltig endast för typ = DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1/) { get; set; } | Hämtar och anger värdet eller uttrycket som är kopplat till villkorlig formatering. |
| [Formula2](../../aspose.cells/formatcondition/formula2/) { get; set; } | Hämtar och anger värdet eller uttrycket som är kopplat till villkorlig formatering. |
| [IconSet](../../aspose.cells/formatcondition/iconset/) { get; } | Hämta den villkorliga formateringens "IconSet"-instans. Standardinstansens IconSetType är TrafficLights31. Giltig endast för typ = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator/) { get; set; } | Hämtar och anger den villkorliga formatoperatorns typ. |
| [Priority](../../aspose.cells/formatcondition/priority/) { get; set; } | Prioriteten för denna villkorliga formateringsregel. Detta värde används för att avgöra vilket format som ska utvärderas och renderas. Lägre numeriska värden har högre prioritet än högre numeriska värden, där '1' är den högsta prioriteten. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue/) { get; set; } | Sant, inga regler med lägre prioritet får tillämpas över denna regel när den utvärderas till sant. Gäller endast för Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style/) { get; set; } | Hämtar eller anger stil för villkorligt formaterade cellområden. |
| [Text](../../aspose.cells/formatcondition/text/) { get; set; } | Textvärdet i en "text contains"-villkorlig formateringsregel. Giltig endast för typ = containsText, notContainsText, beginsWith och endsWith. Standardvärdet är null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod/) { get; set; } | Den tillämpliga tidsperioden i en "date occurrin"-villkorlig formateringsregel. Giltig endast för typ = timePeriod. Standardvärdet är TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10/) { get; } | Hämta den villkorliga formateringens "Top10"-instans. Standardinstansens regel markerar celler vars värden faller inom de 10 bästa. Giltig endast för typ = Top10. |
| [Type](../../aspose.cells/formatcondition/type/) { get; set; } | Hämtar och anger om den villkorliga formattypen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1)(bool, bool) | Hämtar värdet eller uttrycket som är kopplat till detta formatvillkor. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_2)(int, int) | Hämtar formeln för cellens villkorliga formatering. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_1)(bool, bool, int, int) | Hämtar värdet eller uttrycket för cellens villkorliga formatering. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2)(bool, bool) | Hämtar värdet eller uttrycket som är kopplat till detta formatvillkor. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_2)(int, int) | Hämtar formeln för cellens villkorliga formatering. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_1)(bool, bool, int, int) | Hämtar värdet eller uttrycket för cellens villkorliga formatering. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1/)(string, bool, bool) | Anger värdet eller uttrycket som är kopplat till detta formatvillkor. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2/)(string, bool, bool) | Anger värdet eller uttrycket som är kopplat till detta formatvillkor. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas/)(string, string, bool, bool) | Anger värdet eller uttrycket som är kopplat till detta formatvillkor. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionDemo
    {
        public static void FormatConditionExample()
        {
            // Skapa en ny arbetsbok.
            Workbook workbook = new Workbook();

            // Hämta det första kalkylbladet.
            Worksheet sheet = workbook.Worksheets[0];

            // Lägger till en tom villkorlig formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Ställer in det villkorsstyrda formatintervallet.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Lägger till villkor.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            FormatCondition fc = fcs[conditionIndex];

            // Ställa in egenskaper
            fc.Formula1 = "=A2";
            fc.Formula2 = "100";
            fc.Operator = OperatorType.Between;
            fc.StopIfTrue = true;
            fc.Priority = 1;
            fc.Style.BackgroundColor = Color.Red;
            fc.Type = FormatConditionType.CellValue;

            // Visar andra egenskaper
            fc.Text = "Sample Text";
            fc.TimePeriod = TimePeriodType.Today;

            // Sparar Excel-filen
            workbook.Save("FormatConditionExample.xlsx");
            workbook.Save("FormatConditionExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


