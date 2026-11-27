---
title: "IconFilter.IconId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IconFilter egenskap. Hämtar och anger nollbaserat index för en ikon i en ikonuppsättning"
type: docs
url: /sv/net/aspose.cells/iconfilter/iconid/
---
## IconFilter.IconId property

Hämtar och anger nollbaserat index för en ikon i en ikonuppsättning.

```csharp
public int IconId { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconIdDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Tillämpa villkorsstyrd formatering för ikonuppsättning
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.TrafficLights31;
            
            // Ange område med CellArea
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Skapa autofilter med ikonfilter
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;
            
            // Hämta befintligt filter istället för att skapa en ny instans
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 0;

            Console.WriteLine("Current IconId value: " + iconFilter.IconId);

            // Ändra IconId för att filtrera olika ikoner
            iconFilter.IconId = 1;

            workbook.Save("PropertyIconIdDemo.xlsx");
        }
    }
}
```

### Se även

* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


