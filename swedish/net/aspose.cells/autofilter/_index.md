---
title: "Klassen AutoFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AutoFilter-klass. Representerar autofilter för det angivna kalkylbladet"
type: docs
url: /sv/net/aspose.cells/autofilter/
---
## AutoFilter class

Representerar autofilter för det angivna kalkylbladet.

```csharp
public class AutoFilter
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FilterColumns](../../aspose.cells/autofilter/filtercolumns/) { get; } | Hämtar samlingen av filterkolumnerna. |
| [Range](../../aspose.cells/autofilter/range/) { get; set; } | Representerar det område som den angivna AutoFilter gäller för. |
| [ShowFilterButton](../../aspose.cells/autofilter/showfilterbutton/) { get; set; } | Anger om AutoFilter-knappen för den här kolumnen är synlig. |
| [Sorter](../../aspose.cells/autofilter/sorter/) { get; } | Hämtar datasorteringen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddDateFilter](../../aspose.cells/autofilter/adddatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Lägger till ett datumfilter. |
| [AddFillColorFilter](../../aspose.cells/autofilter/addfillcolorfilter/)(int, BackgroundType, CellsColor, CellsColor) | Lägger till ett fyllnadsfärgsfilter. |
| [AddFilter](../../aspose.cells/autofilter/addfilter/)(int, string) | Lägger till ett filter för en filterkolumn. |
| [AddFontColorFilter](../../aspose.cells/autofilter/addfontcolorfilter/)(int, CellsColor) | Lägger till ett teckensnittsfärgsfilter. |
| [AddIconFilter](../../aspose.cells/autofilter/addiconfilter/)(int, IconSetType, int) | Lägger till ett ikonfilter. |
| [Custom](../../aspose.cells/autofilter/custom/#custom)(int, FilterOperatorType, object) | Filtrerar en lista med ett anpassat kriterium. |
| [Custom](../../aspose.cells/autofilter/custom/#custom_1)(int, FilterOperatorType, object, bool, FilterOperatorType, object) | Filtrerar en lista med anpassade kriterier. |
| [DynamicFilter](../../aspose.cells/autofilter/dynamicfilter/)(int, DynamicFilterType) | Lägger till ett dynamiskt filter. |
| [Filter](../../aspose.cells/autofilter/filter/)(int, string) | Filtrerar en lista med specificerade kriterier. |
| [FilterTop10](../../aspose.cells/autofilter/filtertop10/)(int, bool, bool, int) | Filtrera de 10 bästa objekten i listan |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea)() | Hämtar [`CellArea`](../cellarea/) där detta AutoFilter gäller. |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea_1)(bool) | Hämtar [`CellArea`](../cellarea/) där den angivna AutoFilter gäller. |
| [MatchBlanks](../../aspose.cells/autofilter/matchblanks/)(int) | Matcha alla tomma celler i listan. |
| [MatchNonBlanks](../../aspose.cells/autofilter/matchnonblanks/)(int) | Matcha alla icke-tomma celler i listan. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh)() | Uppdatera autofilter för att dölja eller visa raderna. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh_1)(bool) | Hämtar alla dolda raders index. |
| [RemoveDateFilter](../../aspose.cells/autofilter/removedatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Tar bort ett datumfilter. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter)(int) | Ta bort det specifika filtret. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter_1)(int, string) | Tar bort ett filter för en filterkolumn. |
| [SetRange](../../aspose.cells/autofilter/setrange/)(int, int, int) | Ställer in intervallet som den angivna AutoFiltern gäller för. |
| [ShowAll](../../aspose.cells/autofilter/showall/)() | Visa alla rader. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterDemo
    {
        public static void AutoFilterExample()
        {
            // Skapar en filström som innehåller Excel-filen som ska öppnas
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Åtkomst till det första kalkylbladet i Excel-filen
            Worksheet worksheet = workbook.Worksheets[0];
            // Skapar AutoFilter genom att ange cellintervallet för rubrikraden
            worksheet.AutoFilter.Range = "A1:B8";
            // Filtrerar kolumner med angivna värden
            worksheet.AutoFilter.Filter(0, "Bananas");
            worksheet.AutoFilter.Refresh();

            // Sparar den modifierade Excel-filen.
            workbook.Save("AutoFilterExample.xlsx");
            workbook.Save("AutoFilterExample.pdf");

            // Instansiering av ett Workbook-objekt
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Åtkomst till det första kalkylbladet i Excel-filen
            worksheet = workbook.Worksheets[0];

            // Ytterligare kod för att demonstrera andra funktioner i AutoFilter
            // Ställer in intervallet för AutoFilter
            worksheet.AutoFilter.Range = "A1:B8";
            // Lägger till ett filter
            worksheet.AutoFilter.AddFilter(0, "Apples");
            // Lägger till ett datumfilter
            worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);

            worksheet.AutoFilter.Refresh();
            // Sparar den modifierade Excel-filen.
            workbook.Save("AutoFilterExample2.xlsx");
            workbook.Save("AutoFilterExample2.pdf");

            // Instansiering av ett Workbook-objekt
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Åtkomst till det första kalkylbladet i Excel-filen
            worksheet = workbook.Worksheets[0];
                        
            // Lägger till ett teckensnittsfärgsfilter
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Red;

            worksheet.AutoFilter.AddFontColorFilter(0, color);

            worksheet.AutoFilter.Refresh();
            // Sparar den modifierade Excel-filen.
            workbook.Save("AutoFilterExample3.xlsx");
            workbook.Save("AutoFilterExample3.pdf");

            // Instansiering av ett Workbook-objekt
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Åtkomst till det första kalkylbladet i Excel-filen
            worksheet = workbook.Worksheets[0];

            // Lägger till ett fyllningsfärgsfilter
            CellsColor foregroundColor = workbook.CreateCellsColor();
            foregroundColor.Color = System.Drawing.Color.Red;
            CellsColor backgroundColor = workbook.CreateCellsColor();
            backgroundColor.Color = System.Drawing.Color.White;

            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, foregroundColor, backgroundColor);

            worksheet.AutoFilter.Refresh();
            // Sparar den modifierade Excel-filen.
            workbook.Save("AutoFilterExample4.xlsx");
            workbook.Save("AutoFilterExample4.pdf");

            // Instansiering av ett Workbook-objekt
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Åtkomst till det första kalkylbladet i Excel-filen
            worksheet = workbook.Worksheets[0];

            // Matchar tomma
            worksheet.AutoFilter.MatchBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Sparar den modifierade Excel-filen.
            workbook.Save("AutoFilterExample5.xlsx");
            workbook.Save("AutoFilterExample5.pdf");

            // Instansiering av ett Workbook-objekt
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Åtkomst till det första kalkylbladet i Excel-filen
            worksheet = workbook.Worksheets[0];

            // Matchar icke-tomma
            worksheet.AutoFilter.MatchNonBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Sparar den modifierade Excel-filen.
            workbook.Save("AutoFilterExample6.xlsx");
            workbook.Save("AutoFilterExample6.pdf");

            // Instansiering av ett Workbook-objekt
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Åtkomst till det första kalkylbladet i Excel-filen
            worksheet = workbook.Worksheets[0];

            // Anpassat filter
            worksheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "Test");

            worksheet.AutoFilter.Refresh();
            // Sparar den modifierade Excel-filen.
            workbook.Save("AutoFilterExample7.xlsx");
            workbook.Save("AutoFilterExample7.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


