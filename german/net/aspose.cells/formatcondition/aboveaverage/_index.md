---
title: "FormatCondition.AboveAverage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Rufen Sie die AboveAverage-Instanz der bedingten Formatierung ab. Die Standardregel hebt Zellen hervor, die über dem Durchschnitt aller Werte im Bereich liegen. Nur gültig für den Typ AboveAverage."
type: docs
url: /de/net/aspose.cells/formatcondition/aboveaverage/
---
## FormatCondition.AboveAverage property

Rufen Sie die "AboveAverage"-Instanz der bedingten Formatierung ab. Die Regel der Standardinstanz hebt Zellen hervor, die über dem Durchschnitt aller Werte im Bereich liegen. Gültig nur für Typ = AboveAverage.

```csharp
public AboveAverage AboveAverage { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyAboveAverageDemo
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
            worksheet.Cells["A5"].PutValue(50);

            // Bedingte Formatierung für über dem Durchschnitt hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 4, EndColumn = 0 });

            // Festlegen, um Werte über dem Durchschnitt hervorzuheben
            FormatCondition fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = true;
            fc.Style.BackgroundColor = Color.Yellow;

            // Bedingte Formatierung für unter dem Durchschnitt hinzufügen
            index = worksheet.ConditionalFormattings.Add();
            fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.AboveAverage);
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 1, EndRow = 4, EndColumn = 1 });

            // Festlegen, um Werte unter dem Durchschnitt hervorzuheben
            fc = fcc[0];
            fc.AboveAverage.IsAboveAverage = false;
            fc.Style.BackgroundColor = Color.LightBlue;

            // Speichere die Arbeitsmappe
            workbook.Save("AboveAverageConditionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AboveAverage](../../aboveaverage/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


