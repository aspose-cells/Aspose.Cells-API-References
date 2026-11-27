---
title: "IconFilter.IconSetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IconFilter-egenskap. Hämtar och anger vilken ikonuppsättning som används för detta filterkriterium"
type: docs
url: /sv/net/aspose.cells/iconfilter/iconsettype/
---
## IconFilter.IconSetType property

Hämtar och anger vilken ikonuppsättning som används för detta filterkriterium.

```csharp
public IconSetType IconSetType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Skapa autofilter
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;

            // Hämta ikonfiltret
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;

            // Visa aktuell IconSetType (standard är None)
            Console.WriteLine("Current IconSetType: " + iconFilter.IconSetType);

            // Ställ in till 3-pils ikonuppsättning
            iconFilter.IconSetType = IconSetType.Arrows3;
            iconFilter.IconId = 1; // Show only middle arrow

            // Tillämpa villkorsstyrd formatering för att visualisera ikonerna
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.Arrows3;
            
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Byt till trafikljusikonuppsättning
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 2; // Show only green light

            // Spara resultatet
            workbook.Save("PropertyIconSetTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [IconSetType](../../iconsettype/)
* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


