---
title: "Klass LoadFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LoadFilter-klass. Representerar filtret som tillhandahåller alternativ för att läsa in data när arbetsboken laddas från en mall"
type: docs
url: /sv/net/aspose.cells/loadfilter/
---
## LoadFilter class

Representerar filtret som tillhandahåller alternativ för att läsa in data när arbetsboken laddas från en mall.

```csharp
public class LoadFilter
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LoadFilter](loadfilter/#constructor)() | Skapar ett LoadFilter med standardfilteralternativ LoadDataFilterOptions.All. |
| [LoadFilter](loadfilter/#constructor_1)(LoadDataFilterOptions) | Skapar ett LoadFilter med angivna filteralternativ. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions/) { get; set; } | Filteralternativen för att ange vilken data som ska läsas in. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder/) { get; } | Anger vilka blad (index) och i vilken ordning de ska läsas in. Standard är null, vilket betyder att alla blad läses in i standardordning i mallfilen. Om värdet inte är null och ett bladindex inte finns i den returnerade arrayen, kommer bladet inte att läsas in. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet/)(Worksheet) | Förbereder filteralternativ innan det angivna kalkylbladet läses in. Användarens implementation av LoadFilter kan ändra LoadDataFilterOptions här för att ange hur data ska läsas in för detta kalkylblad. |

### Anmärkningar

Användaren kan ange filteralternativen eller implementera sin egen LoadFilter för att ange hur data ska läsas in.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterDemo
    {
        public static void LoadFilterExample()
        {
            // Skapa LoadOptions och ange LoadFilter
            LoadOptions opts = new LoadOptions();
            opts.LoadFilter = new CustomLoadFilter();

            // Läs in arbetsboken med de specificerade LoadOptions
            Workbook wb = new Workbook("LoadFilterExample_original.xlsx", opts);

            // Spara arbetsboken för att se effekten av LoadFilter
            wb.Save("LoadFilterExample.xlsx");
        }

        // Anpassad LoadFilter-implementation
        public class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                if (sheet.Name == "Sheet1")
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.All;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


