---
title: "DataBar.BarFillType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataBar-Eigenschaft. Gibt an oder legt fest, wie eine Datenleiste mit Farbe gefüllt wird"
type: docs
url: /de/net/aspose.cells/databar/barfilltype/
---
## DataBar.BarFillType property

Liest oder legt fest, wie ein Datenbalken mit Farbe gefüllt wird.

```csharp
public DataBarFillType BarFillType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarFillTypeDemo
    {
        public static void Run()
        {
            // Instanziiere ein Workbook-Objekt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Den Bereich der bedingten Formatierung festlegen
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 5,
                StartColumn = 0,
                EndColumn = 5
            };
            fcs.AddArea(ca);

            // Fügen Sie eine DataBar-Bedingung hinzu
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Konfigurieren Sie DataBar-Eigenschaften
            DataBar dataBar = fc.DataBar;
            dataBar.BarFillType = DataBarFillType.Gradient; // Demonstrating BarFillType usage
            dataBar.Color = Color.Blue;

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(100);

            // Speichere die Arbeitsmappe
            workbook.Save("DataBarFillTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [DataBarFillType](../../databarfilltype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


