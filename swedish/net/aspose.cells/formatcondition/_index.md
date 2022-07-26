---
title: FormatCondition
second_title: Aspose.Cells för .NET API-referens
description: Representerar villkorligt formateringsvillkor.
type: docs
weight: 3560
url: /sv/net/aspose.cells/formatcondition/
---
## FormatCondition class

Representerar villkorligt formateringsvillkor.

```csharp
public class FormatCondition
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage) { get; } | Hämta den villkorliga formateringens "AboveAverage"-instans. Standardinstansens regel framhäver celler som är över genomsnittet för alla värden i intervallet. Gäller endast för typ = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale) { get; } | Hämta den villkorliga formateringens "ColorScale"-instans. Standardinstansen är en "grön-gul-röd" 3ColorScale . Gäller endast för typ = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar) { get; } | Hämta den villkorliga formateringens "DataBar"-instans. Standardinstansens färg är blå. Gäller endast för typen är DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1) { get; set; } | Hämtar och ställer in värdet eller uttrycket som är associerat med villkorlig formatering. |
| [Formula2](../../aspose.cells/formatcondition/formula2) { get; set; } | Hämtar och ställer in värdet eller uttrycket som är associerat med villkorlig formatering. |
| [IconSet](../../aspose.cells/formatcondition/iconset) { get; } | Hämta den villkorliga formateringens "IconSet"-instans. Standardinstansens IconSetType är TrafficLights31. Gäller endast för typ = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator) { get; set; } | Hämtar och ställer in den villkorliga formatoperatortypen. |
| [Priority](../../aspose.cells/formatcondition/priority) { get; set; } | Prioriteten för denna villkorliga formateringsregel. Detta värde används för att bestämma vilket -format som ska utvärderas och renderas. Lägre numeriska värden har högre prioritet än högre numeriska värden, där '1' är högsta prioritet. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue) { get; set; } | Sant, inga regler med lägre prioritet får tillämpas över denna regel när denna regel utvärderas till sant. Gäller endast för Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style) { get; set; } | Hämtar eller ställer in stil för villkorligt formaterade cellområden. |
| [Text](../../aspose.cells/formatcondition/text) { get; set; } | Textvärdet i en "text innehåller" villkorlig formateringsregel. Gäller endast för typen = containsText, notContainsText, beginsWith och endsWith. Standardvärdet är null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod) { get; set; } | Tillämplig tidsperiod i en villkorlig formateringsregel "datum inträffar...". Gäller endast för typ = timePeriod. Standardvärdet är TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10) { get; } | Hämta den villkorliga formateringens "Top10"-instans. Standardinstansens regel framhäver celler vars -värden hamnar i topp 10-parentesen. Gäller endast för typen är Top10. |
| [Type](../../aspose.cells/formatcondition/type) { get; set; } | Hämtar och ställer in om det villkorliga formatet Type. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1)(bool, bool) | Hämtar värdet eller uttrycket som är associerat med detta formatvillkor. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_2)(int, int) | Hämtar formeln för den villkorliga formateringen av cellen. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_1)(bool, bool, int, int) | Hämtar värdet eller uttrycket för den villkorliga formateringen av cellen. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2)(bool, bool) | Hämtar värdet eller uttrycket som är associerat med detta formatvillkor. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_2)(int, int) | Hämtar formeln för den villkorliga formateringen av cellen. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_1)(bool, bool, int, int) | Hämtar värdet eller uttrycket för den villkorliga formateringen av cellen. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1)(string, bool, bool) | Anger värdet eller uttrycket som är associerat med detta formatvillkor. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2)(string, bool, bool) | Anger värdet eller uttrycket som är associerat med detta formatvillkor. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas)(string, string, bool, bool) | Anger värdet eller uttrycket som är associerat med detta formatvillkor. |

### Exempel

```csharp

[C#]
//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
 
//Lägger till en tom villkorlig formatering
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
 
//Ställer in det villkorliga formatintervallet.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
 
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);
 
//Lägger till villkor.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
 
//Lägger till villkor.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
 
//Ställer in bakgrundsfärgen.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
 
//Spara Excel-filen
workbook.Save("output.xls");

[VB.NET]

'Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()
Dim sheet As Worksheet = workbook.Worksheets(0)
 
' Lägger till en tom villkorlig formatering
Dim index As Integer = sheet.ConditionalFormattings.Add()
Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)
 
'Ställer in det villkorliga formatintervallet.
Dim ca As CellArea = New CellArea()
ca.StartRow = 0
ca.EndRow = 0
ca.StartColumn = 0
ca.EndColumn = 0
fcs.AddArea(ca)
ca = New CellArea()
ca.StartRow = 1
ca.EndRow = 1
ca.StartColumn = 1
ca.EndColumn = 1
fcs.AddArea(ca)
 
'Lägger till skick.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")
 
'Lägger till skick.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")
 
'Ställer in bakgrundsfärgen.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
 
'Sparar Excel-filen
workbook.Save("output.xls")
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
