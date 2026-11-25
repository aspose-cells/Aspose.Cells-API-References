---
title: "DataBar.MaxLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBar. Rappresenta la lunghezza massima della barra dati"
type: docs
url: /it/net/aspose.cells/databar/maxlength/
---
## DataBar.MaxLength property

Rappresenta la lunghezza massima della DataBar.

```csharp
public int MaxLength { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Aggiungi formattazione condizionale
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
            
            CellArea area = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(area);

            // Aggiungi barra dati e imposta le proprietà
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;
            
            dataBar.Color = Color.Blue;
            dataBar.MinLength = 0;
            dataBar.MaxLength = 90; // Demonstrating MaxLength property
            
            workbook.Save("DataBarMaxLengthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


