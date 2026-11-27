---
title: "HtmlSaveOptions.SheetSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Hämtar eller anger vilka blad som ska renderas. Standard är alla synliga blad i arbetsboken Visible"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/sheetset/
---
## HtmlSaveOptions.SheetSet property

Hämtar eller anger vilka blad som ska renderas. Standard är alla synliga blad i arbetsboken: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med flera kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Gör ett blad dolt för demonstration
            workbook.Worksheets[1].IsVisible = false;

            // Ställ in exempeldata i varje blad
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from {sheet.Name}");
            }

            // Skapa en HtmlSaveOptions-instans
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Visa aktuellt SheetSet‑värde (standard är null vilket betyder alla synliga blad)
            Console.WriteLine("Current SheetSet value: " + (options.SheetSet == null ? "All visible sheets" : "Custom set"));

            // Ställ in SheetSet för att endast inkludera specifika blad (efter index)
            options.SheetSet = new SheetSet(new int[] { 0, 2 });

            // Spara till HTML – endast de angivna bladen kommer att inkluderas
            workbook.Save("HtmlWithCustomSheetSet.html", options);

            // Ändra SheetSet till endast synliga blad
            options.SheetSet = SheetSet.Visible;
            workbook.Save("HtmlWithVisibleSheets.html", options);

            // Ändra SheetSet till endast aktivt blad
            workbook.Worksheets[2].IsSelected = true; // Activate the sheet by selecting it
            options.SheetSet = SheetSet.Active;
            workbook.Save("HtmlWithActiveSheet.html", options);
        }
    }
}
```

### Se även

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


