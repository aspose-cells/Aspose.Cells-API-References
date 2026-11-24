---
title: "DataLabels.SeparatorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt den Trennzeichen-Typ zurück, der für die Datenbeschriftungen in einem Diagramm verwendet wird, oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/datalabels/separatortype/
---
## DataLabels.SeparatorType property

Liest oder legt den Trennertyp fest, der für die Datenlabels in einem Diagramm verwendet wird.

```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```

### Hinweise

Um ein benutzerdefiniertes Trennzeichen festzulegen, setzen Sie bitte die Eigenschaft `SeparatorType` auf Custom und geben dann den erwarteten Wert für [`SeparatorValue`](../separatorvalue/) an.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen aktivieren
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            
            // Trennzeichen-Typ festlegen
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Space;

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsSeparatorTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


