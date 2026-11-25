---
title: "DataBar.MinLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBar. Rappresenta la lunghezza minima della barra dati"
type: docs
url: /it/net/aspose.cells/databar/minlength/
---
## DataBar.MinLength property

Rappresenta la lunghezza minima della DataBar.

```csharp
public int MinLength { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            worksheet.Cells["A3"].PutValue(25);
            worksheet.Cells["A4"].PutValue(35);

            // Aggiungi formattazione condizionale
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

            // Aggiungi barra dati
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            DataBar dataBar = fc.DataBar;

            // Configura barra dati
            dataBar.Color = Color.Green;
            dataBar.MinLength = 10;  // Minimum length set to 10%
            dataBar.MaxLength = 100;

            workbook.Save("DataBarMinLengthDemo.xlsx");
            Console.WriteLine("DataBar with MinLength demo executed successfully.");
        }
    }
}
```

### Vedi anche

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


