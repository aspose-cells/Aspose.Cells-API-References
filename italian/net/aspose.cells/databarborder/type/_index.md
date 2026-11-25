---
title: "DataBarBorder.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBarBorder. Ottiene o imposta il tipo di bordo delle barre dati specificate da una regola di formattazione condizionale"
type: docs
url: /it/net/aspose.cells/databarborder/type/
---
## DataBarBorder.Type property

Ottiene o imposta il tipo del bordo delle barre dei dati specificato da una regola di formattazione condizionale.

```csharp
public DataBarBorderType Type { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarBorderPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            DataBar dataBar = fc.DataBar;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Red;

            workbook.Save("DataBarBorderTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* enum [DataBarBorderType](../../databarbordertype/)
* class [DataBarBorder](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


