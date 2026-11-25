---
title: "FormatConditionCollection.RangeCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormatConditionCollection. Ottiene il conteggio degli intervalli formattati condizionalmente"
type: docs
url: /it/net/aspose.cells/formatconditioncollection/rangecount/
---
## FormatConditionCollection.RangeCount property

Ottiene il conteggio degli intervalli formattati condizionalmente.

```csharp
public int RangeCount { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyRangeCountDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Aggiungi formattazione condizionale
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Aggiungi intervalli usando il metodo AddArea invece di AddRange
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 3, EndColumn = 0 });
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "50");

            // Dimostra la proprietà RangeCount
            Console.WriteLine($"Number of ranges in FormatConditionCollection: {fcc.RangeCount}");
            
            // Convalida RangeCount
            if (fcc.RangeCount < 1)
            {
                Console.WriteLine("Error: No ranges applied to conditional formatting");
            }
            else
            {
                Console.WriteLine("Conditional formatting ranges applied successfully");
            }
        }
    }
}
```

### Vedi anche

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


