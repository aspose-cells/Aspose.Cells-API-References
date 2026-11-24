---
title: "Klasse AboveAverage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AboveAverage Klasse. Beschreibt die AboveAverage‑Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel hebt Zellen hervor, die über oder unter dem Durchschnitt aller Werte im Bereich liegen."
type: docs
url: /de/net/aspose.cells/aboveaverage/
---
## AboveAverage class

Beschreiben Sie die AboveAverage-Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel hebt Zellen hervor, die über oder unter dem Durchschnitt aller Werte im Bereich liegen.

```csharp
public class AboveAverage
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [AboveAverage](aboveaverage/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsAboveAverage](../../aspose.cells/aboveaverage/isaboveaverage/) { get; set; } | Lese oder setze das Flag, das angibt, ob die Regel eine „above average“-Regel ist. 'true' bedeutet 'above average'. Standardwert ist true. |
| [IsEqualAverage](../../aspose.cells/aboveaverage/isequalaverage/) { get; set; } | Lese oder setze das Flag, das angibt, ob die Kriterien 'aboveAverage' und 'belowAverage' den Durchschnittswert einschließen oder ausschließen. 'true' bedeutet, den Durchschnittswert in die Kriterien einzubeziehen. Standardwert ist false. |
| [StdDev](../../aspose.cells/aboveaverage/stddev/) { get; set; } | Lese oder setze die Anzahl der Standardabweichungen, die über oder unter dem Durchschnitt in der bedingten Formatierungsregel berücksichtigt werden sollen. Der Eingabewert muss zwischen 0 und 3 liegen (inklusive 0 und 3). Wird dieser Wert auf 0 gesetzt, ist stdDev nicht festgelegt. Der Standardwert ist 0. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class AboveAverageDemo
    {
        public static void AboveAverageExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            // Eine bedingte Formatierungssammlung zum Arbeitsblatt hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            // Definiere den Zellbereich, auf den die bedingte Formatierung angewendet wird
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Eine above average‑Bedingung zur Sammlung hinzufügen
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            // Setze die Hintergrundfarbe für die Bedingung
            fc.Style.BackgroundColor = Color.Yellow;

            // Setze Eigenschaften für die above average‑Bedingung
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            Cells cells = worksheet.Cells;
            cells["A1"].Value = 20;
            cells["A2"].Value = 300;
            cells["A3"].Value = 40;
            cells["A4"].Value = 500;
            cells["A5"].Value = 6;
            cells["A6"].Value = 70;
            cells["A7"].Value = 8;
            cells["A8"].Value = 900;
            cells["A9"].Value = 10;

            cells["C1"].Value = 2;
            cells["C2"].Value = 3;
            cells["C3"].Value = 4;
            cells["C4"].Value = 5;
            cells["C5"].Value = 3;
            cells["C6"].Value = 2;
            cells["C7"].Value = 8;
            cells["C8"].Value = 300;
            cells["C9"].Value = 10;

            // Speichere die Arbeitsmappe
            workbook.Save("AboveAverageExample.xlsx");
            workbook.Save("AboveAverageExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


