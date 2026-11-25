---
title: "SparklineGroup.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Indica il tipo di sparkline del gruppo di sparklines"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/type/
---
## SparklineGroup.Type property

Indica il tipo di sparkline del gruppo di sparkline.

```csharp
public SparklineType Type { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Crea un gruppo di sparklines con tipo Colonna
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Column, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Cambia il tipo di sparkline in Linea
            group.Type = SparklineType.Line;

            // Aggiungi la sparkline al gruppo
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Salva la cartella di lavoro
            workbook.Save("SparklineTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


