---
title: "Klass FindOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FindOptions klass. Representerar sökalternativ"
type: docs
url: /sv/net/aspose.cells/findoptions/
---
## FindOptions class

Representerar sökalternativ.

```csharp
public class FindOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [FindOptions](findoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive/) { get; set; } | Indikerar om den sökta strängen är skiftlägeskänslig. |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata/) { get; set; } | Hämtar eller anger ett värde som indikerar om den sökta strängvärdet ska konverteras till numerisk data. |
| [IsCaseSensitive](../../aspose.cells/findoptions/iscasesensitive/) { get; set; } | (**Obsolete.**) Indikerar om den sökta strängen är skiftlägeskänslig. |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset/) { get; } | Anger om det sökta intervallet är angivet. |
| [LookAtType](../../aspose.cells/findoptions/lookattype/) { get; set; } | Titta på typen. |
| [LookInType](../../aspose.cells/findoptions/lookintype/) { get; set; } | Titta i typen. |
| [RegexKey](../../aspose.cells/findoptions/regexkey/) { get; set; } | Anger om den sökta nyckeln är ett regex. Om true kommer den sökta nyckeln att behandlas som regex och tolkas. Annars kommer nyckeln att tolkas enligt reglerna i MS Excel. |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward/) { get; set; } | Om sökningen ska gå bakåt för celler. |
| [SearchNext](../../aspose.cells/findoptions/searchnext/) { get; set; } | (**Obsolete.**) Sökordning. True: sök nästa. False: sök föregående. |
| [SearchOrderByRows](../../aspose.cells/findoptions/searchorderbyrows/) { get; set; } | Anger om sökordningen är efter rader eller kolumner. |
| [Style](../../aspose.cells/findoptions/style/) { get; set; } | Formatet att söka efter. |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive/) { get; set; } | Anger om den sökta cellvärdestypen ska vara densamma som den sökta nyckeln. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange/)() | Hämtar och anger det sökta intervallet. |
| [SetRange](../../aspose.cells/findoptions/setrange/)(CellArea) | Anger det sökta intervallet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsDemo
    {
        public static void FindOptionsExample()
        {
            // Instansiera arbetsbokobjektet
            Workbook workbook = new Workbook("FindOptionsExample_original.xlsx");

            // Hämta Cells-samlingen 
            Cells cells = workbook.Worksheets[0].Cells;

            // Instansiera FindOptions-objektet
            FindOptions findOptions = new FindOptions();

            // Skapa ett Cells-område
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 5;
            ca.EndColumn = 5;

            // Ställ in cellområdet för sökalternativ
            findOptions.SetRange(ca);

            // Ställ in sökegenskaper
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Hitta cellen med värdet 0
            Cell cell = cells.Find(0, null, findOptions);

            if (cell != null)
            {
                Console.WriteLine("Cell found at: " + cell.Name);
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


