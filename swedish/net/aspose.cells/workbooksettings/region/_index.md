---
title: "WorkbookSettings.Region"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings‑egenskap. Hämtar eller anger de regionala inställningarna för arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

Hämtar eller anger de regionala inställningarna för arbetsboken.

```csharp
public CountryCode Region { get; set; }
```

### Anmärkningar

1. Regionala inställningar som används av Aspose.Cells‑komponenten för en arbetsbok som laddas från en mallfil: i). För en XLS‑fil finns fält definierade för regionala inställningar och MS Excel sparar regionala inställningsdata i filen när XLS‑filen sparas. Därför använder vi den sparade regionen i mallfilen för arbetsboken. Om du inte vill använda den region som sparats i XLS‑filen, återställ den till den förväntade (t.ex. CountryCode.Default) efter att ha laddat mallfilen. Dessutom sparar vi det användarspecificerade värdet (med denna metod) i filen när en XLS‑fil sparas. ii). För andra filformat, såsom XLSX, XLSB… osv., finns inget fält definierat för regionala inställningar i filformatsspecifikationen. Därför använder vi de regionala inställningarna från applikationens miljö för arbetsboken. Och det användarspecificerade värdet (med denna metod) kan inte bevaras för de genererade filerna med dessa format. 2. För visningseffekten i MS Excel: De tillämpade regionala inställningarna här kan bara träda i kraft vid körning med Aspose.Cells‑komponenten och inte när den genererade filen visas i MS Excel. Även för den genererade XLS‑filen där de specificerade regionala inställningsdata har sparats, så använder MS Excel alltid den standardregionala inställningen i den miljö där MS Excel körs när filen visas/redigeras, inte den som sparats i filen. Detta är MS Excels beteende och kan inte ändras med kod.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRegionDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Japan;
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(44089); // Represents 2020-09-15
            
            Style style = cell.GetStyle();
            style.Custom = "[$-F800]yyyy年m月d日";
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Se även

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


