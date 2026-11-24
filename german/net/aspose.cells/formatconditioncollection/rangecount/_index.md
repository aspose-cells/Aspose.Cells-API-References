---
title: "FormatConditionCollection.RangeCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatConditionCollection-Eigenschaft. Gibt die Anzahl der bedingt formatierten Bereiche zurück"
type: docs
url: /de/net/aspose.cells/formatconditioncollection/rangecount/
---
## FormatConditionCollection.RangeCount property

Gibt die Anzahl der bedingt formatierten Bereiche zurück.

```csharp
public int RangeCount { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyRangeCountDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Bereiche mit der AddArea-Methode anstelle von AddRange hinzufügen
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 3, EndColumn = 0 });
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "50");

            // RangeCount-Eigenschaft demonstrieren
            Console.WriteLine($"Number of ranges in FormatConditionCollection: {fcc.RangeCount}");
            
            // RangeCount validieren
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

### Siehe auch

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


