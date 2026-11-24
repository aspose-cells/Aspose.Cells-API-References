---
title: "Top10Filter.Criteria"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Top10Filter-Eigenschaft. Der tatsächliche Zellenwert im Bereich, der für den Vergleich dieses Filters verwendet wird. Dies ist der Zwischenspeicherwert während des Aktualisierungsvorgangs"
type: docs
url: /de/net/aspose.cells/top10filter/criteria/
---
## Top10Filter.Criteria property

Der tatsächliche Zellenwert im Bereich, der für den Vergleich dieses Filters verwendet wird. Dies ist der Zwischenspeicherwert während des Aktualisierungsvorgangs.

```csharp
[Obsolete("Ignore this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Criteria { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen ignorieren Sie bitte diese Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Oktober 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class Top10FilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[i, 0].PutValue(20 - i);
            }
            
            worksheet.AutoFilter.Range = "A1:A20";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Korrektur: Auf die Filter‑Eigenschaft zugreifen und zu Top10Filter casten
            Top10Filter filter = (Top10Filter)worksheet.AutoFilter.FilterColumns[0].Filter;
            Console.WriteLine("Current Criteria value: " + filter.Criteria);
            
            filter.Criteria = 14;
            
            worksheet.AutoFilter.Refresh();
            
            workbook.Save("Top10FilterCriteriaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


