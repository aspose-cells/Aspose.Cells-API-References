---
title: "Klasse FormatCondition"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Klasse Aspose.Cells.FormatCondition. Stellt eine bedingte Formatierungsbedingung dar"
type: docs
url: /de/net/aspose.cells/formatcondition/
---
## FormatCondition class

Stellt eine Bedingung für die bedingte Formatierung dar.

```csharp
public class FormatCondition
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage/) { get; } | Rufen Sie die "AboveAverage"-Instanz der bedingten Formatierung ab. Die Regel der Standardinstanz hebt Zellen hervor, die über dem Durchschnitt aller Werte im Bereich liegen. Gültig nur für Typ = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale/) { get; } | Rufen Sie die "ColorScale"-Instanz der bedingten Formatierung ab. Die Standardinstanz ist ein "grün-gelb-rot" 3ColorScale. Gültig nur für Typ = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar/) { get; } | Rufen Sie die "DataBar"-Instanz der bedingten Formatierung ab. Die Farbe der Standardinstanz ist blau. Gültig nur für Typ = DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1/) { get; set; } | Liest und setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| [Formula2](../../aspose.cells/formatcondition/formula2/) { get; set; } | Liest und setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| [IconSet](../../aspose.cells/formatcondition/iconset/) { get; } | Rufen Sie die "IconSet"-Instanz der bedingten Formatierung ab. Der IconSetType der Standardinstanz ist TrafficLights31. Gültig nur für Typ = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator/) { get; set; } | Liest und setzt den Operator-Typ der bedingten Formatierung. |
| [Priority](../../aspose.cells/formatcondition/priority/) { get; set; } | Die Priorität dieser Regel für bedingte Formatierung. Dieser Wert wird verwendet, um zu bestimmen, welches Format ausgewertet und gerendert werden soll. Niedrigere numerische Werte haben höhere Priorität als höhere numerische Werte, wobei '1' die höchste Priorität hat. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue/) { get; set; } | True, es dürfen keine Regeln mit niedrigerer Priorität über diese Regel angewendet werden, wenn diese Regel zu true evaluiert. Gilt nur für Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style/) { get; set; } | Liest oder setzt den Stil von bedingt formatierten Zellbereichen. |
| [Text](../../aspose.cells/formatcondition/text/) { get; set; } | Der Textwert in einer "text contains"-Regel für bedingte Formatierung. Gültig nur für Typ = containsText, notContainsText, beginsWith und endsWith. Der Standardwert ist null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod/) { get; set; } | Der anwendbare Zeitraum in einer "date occurrin"-Regel für bedingte Formatierung. Gültig nur für Typ = timePeriod. Der Standardwert ist TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10/) { get; } | Rufen Sie die "Top10"-Instanz der bedingten Formatierung ab. Die Regel der Standardinstanz hebt Zellen hervor, deren Werte in die Top‑10‑Kategorie fallen. Gültig nur für Typ = Top10. |
| [Type](../../aspose.cells/formatcondition/type/) { get; set; } | Liest und setzt, ob der Typ der bedingten Formatierung gesetzt ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1)(bool, bool) | Liest den Wert oder Ausdruck, der mit dieser Formatierungsbedingung verknüpft ist. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_2)(int, int) | Liest die Formel der bedingten Formatierung der Zelle. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_1)(bool, bool, int, int) | Liest den Wert oder Ausdruck der bedingten Formatierung der Zelle. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2)(bool, bool) | Liest den Wert oder Ausdruck, der mit dieser Formatierungsbedingung verknüpft ist. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_2)(int, int) | Liest die Formel der bedingten Formatierung der Zelle. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_1)(bool, bool, int, int) | Liest den Wert oder Ausdruck der bedingten Formatierung der Zelle. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1/)(string, bool, bool) | Setzt den Wert oder Ausdruck, der mit dieser Formatierungsbedingung verknüpft ist. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2/)(string, bool, bool) | Setzt den Wert oder Ausdruck, der mit dieser Formatierungsbedingung verknüpft ist. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas/)(string, string, bool, bool) | Setzt den Wert oder Ausdruck, der mit dieser Formatierungsbedingung verknüpft ist. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch.
            Workbook workbook = new Workbook();

            // Hole das erste Arbeitsblatt.
            Worksheet sheet = workbook.Worksheets[0];

            // Fügt eine leere bedingte Formatierung hinzu
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Setzt den Bereich für die bedingte Formatierung.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Fügt Bedingung hinzu.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            FormatCondition fc = fcs[conditionIndex];

            // Eigenschaften festlegen
            fc.Formula1 = "=A2";
            fc.Formula2 = "100";
            fc.Operator = OperatorType.Between;
            fc.StopIfTrue = true;
            fc.Priority = 1;
            fc.Style.BackgroundColor = Color.Red;
            fc.Type = FormatConditionType.CellValue;

            // Demonstration weiterer Eigenschaften
            fc.Text = "Sample Text";
            fc.TimePeriod = TimePeriodType.Today;

            // Die Excel-Datei speichern
            workbook.Save("FormatConditionExample.xlsx");
            workbook.Save("FormatConditionExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


