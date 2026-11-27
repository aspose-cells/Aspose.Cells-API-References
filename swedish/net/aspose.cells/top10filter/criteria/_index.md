---
title: "Top10Filter.Criteria"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Top10Filter-egenskap. Det faktiska cellvärdet i intervallet som används för att utföra jämförelsen för detta filter. Detta är cachevärdet under uppdateringsprocessen."
type: docs
url: /sv/net/aspose.cells/top10filter/criteria/
---
## Top10Filter.Criteria property

Det faktiska cellvärdet i intervallet som används för att utföra jämförelsen för detta filter. Detta är cachevärdet under uppdateringsprocessen.

```csharp
[Obsolete("Ignore this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Criteria { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Ignorera istället denna egenskap. Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            
            // Åtgärd: Åtkomst till Filter-egenskap och kasta till Top10Filter
            Top10Filter filter = (Top10Filter)worksheet.AutoFilter.FilterColumns[0].Filter;
            Console.WriteLine("Current Criteria value: " + filter.Criteria);
            
            filter.Criteria = 14;
            
            worksheet.AutoFilter.Refresh();
            
            workbook.Save("Top10FilterCriteriaDemo.xlsx");
        }
    }
}
```

### Se även

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


