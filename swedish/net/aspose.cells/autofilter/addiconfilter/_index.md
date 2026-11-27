---
title: "AutoFilter.AddIconFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Lägger till ett ikonfilter"
type: docs
url: /sv/net/aspose.cells/autofilter/addiconfilter/
---
## AutoFilter.AddIconFilter method

Lägger till ett ikonfilter.

```csharp
public void AddIconFilter(int fieldIndex, IconSetType iconSetType, int iconId)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| iconSetType | IconSetType | Ikonsetttypen. |
| iconId | Int32 | Ikon-id-et. |

### Anmärkningar

Stöder endast att lägga till ikonfilter. Stöder inte att kontrollera vilken rad som är synlig om filtret är ett ikonfilter.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i exempeldata i kolumn A
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);
            cell = worksheet.Cells["B1"];
            cell.PutValue("Values2");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(1, 0, 5, 1));
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];

            // Hämta automatisk filterinstans
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Ställ in autofilterintervall (A1:A6) med startRow, startColumn, endRow
            autoFilter.SetRange(0, 0, 1);

            try
            {
                // Lägg till ikonfilter i första kolumnen (fieldIndex: 0)
                // Använder 3-signalikonset (IconSetType.TrafficLights31)
                // Filtrerar efter första ikonen i setet (iconId: 0)
                autoFilter.AddIconFilter(0, IconSetType.TrafficLights31, 0);
                
                // Uppdatera filter för att tillämpa ändringar
                autoFilter.Refresh();

                Console.WriteLine("Added icon filter to column A showing items with first traffic light icon");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddIconFilter: {ex.Message}");
            }

            // Spara den modifierade arbetsboken
            workbook.Save("AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo.xlsx");
        }
    }
}
```

### Se även

* enum [IconSetType](../../iconsettype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


