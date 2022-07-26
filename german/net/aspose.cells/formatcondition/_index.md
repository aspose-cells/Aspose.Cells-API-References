---
title: FormatCondition
second_title: Aspose.Cells für .NET-API-Referenz
description: Stellt die bedingte Formatierungsbedingung dar.
type: docs
weight: 3560
url: /de/net/aspose.cells/formatcondition/
---
## FormatCondition class

Stellt die bedingte Formatierungsbedingung dar.

```csharp
public class FormatCondition
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage) { get; } | Abrufen der „AboveAverage“-Instanz der bedingten Formatierung. Die Regel der Standardinstanz hebt Zellen hervor, die über dem Durchschnitt aller Werte im Bereich liegen. Nur gültig für type = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale) { get; } | Abrufen der „ColorScale“-Instanz der bedingten Formatierung. Die Standardinstanz ist eine „grün-gelb-rote“ 3ColorScale . Nur gültig für type = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar) { get; } | Abrufen der „DataBar“-Instanz der bedingten Formatierung. Die Farbe der Standardinstanz ist blau. Gültig nur für den Typ DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1) { get; set; } | Ruft den Wert oder Ausdruck ab, der der bedingten Formatierung zugeordnet ist, und legt ihn fest. |
| [Formula2](../../aspose.cells/formatcondition/formula2) { get; set; } | Ruft den Wert oder Ausdruck ab, der der bedingten Formatierung zugeordnet ist, und legt ihn fest. |
| [IconSet](../../aspose.cells/formatcondition/iconset) { get; } | Abrufen der „IconSet“-Instanz der bedingten Formatierung. Der IconSetType der Standardinstanz ist TrafficLights31. Nur gültig für type = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator) { get; set; } | Ruft den Typ des bedingten Formatoperators ab und legt ihn fest. |
| [Priority](../../aspose.cells/formatcondition/priority) { get; set; } | Die Priorität dieser Regel zur bedingten Formatierung. Dieser Wert wird verwendet, um zu bestimmen, welches -Format ausgewertet und gerendert werden soll. Niedrigere numerische Werte haben eine höhere Priorität als höhere numerische Werte, wobei „1“ die höchste Priorität ist. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue) { get; set; } | True, keine Regeln mit niedrigerer Priorität können über diese Regel angewendet werden, wenn diese Regel als wahr ausgewertet wird. Gilt nur für Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style) { get; set; } | Ruft den Stil von bedingt formatierten Zellbereichen ab oder legt ihn fest. |
| [Text](../../aspose.cells/formatcondition/text) { get; set; } | Der Textwert in einer bedingten Formatierungsregel "Text enthält". Nur gültig für type = containsText, notContainsText, beginWith und endedWith. Der Standardwert ist null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod) { get; set; } | Der anwendbare Zeitraum in einer bedingten Formatierungsregel „Datum auftritt…“. Nur gültig für type = timePeriod. Der Standardwert ist TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10) { get; } | Abrufen der „Top10“-Instanz der bedingten Formatierung. Die Regel der Standardinstanz hebt Zellen hervor, deren Werte in die obersten 10 Klammern fallen. Nur gültig für den Typ „Top10“. |
| [Type](../../aspose.cells/formatcondition/type) { get; set; } | Ruft ab und legt fest, ob das bedingte Format Type. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1)(bool, bool) | Ruft den Wert oder Ausdruck ab, der dieser Formatbedingung zugeordnet ist. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_2)(int, int) | Ruft die Formel der bedingten Formatierung der Zelle ab. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_1)(bool, bool, int, int) | Ruft den Wert oder Ausdruck der bedingten Formatierung der Zelle ab. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2)(bool, bool) | Ruft den Wert oder Ausdruck ab, der dieser Formatbedingung zugeordnet ist. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_2)(int, int) | Ruft die Formel der bedingten Formatierung der Zelle ab. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_1)(bool, bool, int, int) | Ruft den Wert oder Ausdruck der bedingten Formatierung der Zelle ab. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1)(string, bool, bool) | Legt den Wert oder Ausdruck fest, der dieser Formatbedingung zugeordnet ist. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2)(string, bool, bool) | Legt den Wert oder Ausdruck fest, der dieser Formatbedingung zugeordnet ist. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas)(string, string, bool, bool) | Legt den Wert oder Ausdruck fest, der dieser Formatbedingung zugeordnet ist. |

### Beispiele

```csharp

[C#]
//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
 
//Fügt eine leere bedingte Formatierung hinzu
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
 
//Legt den bedingten Formatbereich fest.
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
 
//Bedingung hinzufügen.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
 
//Bedingung hinzufügen.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
 
//Setzt die Hintergrundfarbe.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
 
//Speichern der Excel-Datei
workbook.Save("output.xls");

[VB.NET]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()
Dim sheet As Worksheet = workbook.Worksheets(0)
 
' Fügt eine leere bedingte Formatierung hinzu
Dim index As Integer = sheet.ConditionalFormattings.Add()
Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)
 
'Legt den bedingten Formatbereich fest.
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
 
'Fügt Bedingung hinzu.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")
 
'Fügt Bedingung hinzu.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")
 
'Legt die Hintergrundfarbe fest.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
 
'Speichern der Excel-Datei
workbook.Save("output.xls")
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
