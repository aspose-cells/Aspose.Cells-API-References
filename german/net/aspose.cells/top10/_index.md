---
title: "Klasse Top10"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Top10 Klasse. Beschreiben Sie die Top10‑Bedingte‑Formatierungsregel. Diese bedingte Formatierungsregel hebt Zellen hervor, deren Werte im angegebenen oberen N‑ oder unteren N‑Bereich liegen."
type: docs
url: /de/net/aspose.cells/top10/
---
## Top10 class

Beschreiben Sie die Top10‑Bedingte‑Formatierungsregel. Diese bedingte Formatierungsregel hebt Zellen hervor, deren Werte im obersten N‑ oder untersten N‑Bereich liegen, wie angegeben.

```csharp
public class Top10
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Top10](top10/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom/) { get; set; } | Abrufen oder Festlegen, ob eine „top/bottom n“-Regel eine „bottom n“-Regel ist. Standardwert ist false. |
| [IsPercent](../../aspose.cells/top10/ispercent/) { get; set; } | Abrufen oder Festlegen, ob eine „top/bottom n“-Regel eine „top/bottom n percent“-Regel ist. Standardwert ist false. |
| [Rank](../../aspose.cells/top10/rank/) { get; set; } | Abrufen oder Festlegen des Werts von „n“ in einer „top/bottom n“-Bedingten‑Formatierungsregel. Wenn IsPercent true ist, muss der Wert zwischen 0 und 100 liegen. Andernfalls muss er zwischen 0 und 1000 liegen. Standardwert ist 10. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class Top10Demo
    {
        public static void Top10Example()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügt eine leere bedingte Formatierung hinzu
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Setzt den Bereich der bedingten Formatierung
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Fügt Bedingung hinzu
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Eigenschaften festlegen
            Top10 top10 = fc.Top10;
            top10.IsPercent = false;
            top10.IsBottom = false;
            top10.Rank = 5;

            // Die Excel-Datei speichern
            workbook.Save("Top10Example.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


