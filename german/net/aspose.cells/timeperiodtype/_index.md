---
title: "Aufzählung TimePeriodType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TimePeriodType Aufzählung. Wird in einer FormatConditionType.TimePeriod-Bedingten Formatierungsregel verwendet. Dies sind dynamische Zeiträume, die sich basierend auf dem Datum ändern, an dem die bedingte Formatierung aktualisiert / angewendet wird."
type: docs
url: /de/net/aspose.cells/timeperiodtype/
---
## TimePeriodType enumeration

Wird in einer FormatConditionType.TimePeriod‑Bedingten Formatierungsregel verwendet. Dies sind dynamische Zeiträume, die sich basierend auf dem Datum ändern, an dem die bedingte Formatierung aktualisiert / angewendet wird.

```csharp
public enum TimePeriodType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Today | `0` | Heutiges Datum. |
| Yesterday | `1` | Gesternes Datum. |
| Tomorrow | `2` | Morgiges Datum. |
| Last7Days | `3` | Ein Datum in den letzten sieben Tagen. |
| ThisMonth | `4` | Ein Datum, das in diesem Kalendermonat auftritt. |
| LastMonth | `5` | Ein Datum, das im letzten Kalendermonat auftritt. |
| NextMonth | `6` | Ein Datum, das im nächsten Kalendermonat auftritt. |
| ThisWeek | `7` | Ein Datum, das diese Woche auftritt. |
| LastWeek | `8` | Ein Datum, das letzte Woche auftritt. |
| NextWeek | `9` | Ein Datum, das nächste Woche auftritt. |
| ThisYear | `10` | Ein Datum, das dieses Jahr auftritt. Nur für .ods. |
| LastYear | `11` | Ein Datum, das letztes Jahr auftritt. Nur für .ods. |
| NextYear | `12` | Ein Datum, das nächstes Jahr auftritt. Nur für .ods. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TimePeriodTypeDemo
    {
        public static void TimePeriodTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine bedingte Formatierungsregel hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Den Zellbereich für die bedingte Formatierung definieren
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Eine Bedingung für den Zeitraum hinzufügen
            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;

            // Den Zeitraumtyp festlegen
            fc.TimePeriod = TimePeriodType.Today;

            // Speichere die Arbeitsmappe
            workbook.Save("TimePeriodTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


