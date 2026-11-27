---
title: "Enum LoadDataFilterOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LoadDataFilterOptions enum. Representerar alternativen för att filtrera data när arbetsbok laddas från mall"
type: docs
url: /sv/net/aspose.cells/loaddatafilteroptions/
---
## LoadDataFilterOptions enumeration

Representerar alternativen för att filtrera data när arbetsboken laddas från en mall.

```csharp
public enum LoadDataFilterOptions
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Läs in inget för bladdata |
| All | `2147483647` | Läs in allt |
| CellBlank | `1` | Läs in celler vars värde är tomt |
| CellString | `2` | Läs in celler vars värde är en sträng |
| CellNumeric | `4` | Läs in celler vars värde är numeriskt(inklusive datum/tid) |
| CellError | `8` | Läs in celler vars värde är fel |
| CellBool | `16` | Läs in celler vars värde är boolesk |
| CellValue | `31` | Läs in cellvärden (alla värdetyper) endast |
| Formula | `32` | Läs in cellformler. |
| CellData | `67108927` | Läs in celldata inklusive värden, formler och formatering |
| Chart | `256` | Läs in diagram |
| Shape | `402653696` | Läs in former |
| Drawing | `402653952` | Ritobjekt(inklusive Diagram, Bild, OleObject och alla andra ritobjekt) |
| MergedArea | `1024` | Läs in sammanslagna celler |
| ConditionalFormatting | `2048` | Läs in villkorsstyrd formatering |
| DataValidation | `4096` | Läs in datavalideringar |
| PivotTable | `8192` | Läs in pivottabeller |
| Table | `16384` | Läs in tabeller |
| Hyperlinks | `32768` | Läs in hyperlänkar |
| SheetSettings | `65536` | Läs in inställningar för arbetsblad |
| SheetData | `403701759` | Läs in all data för arbetsblad, såsom celldata, inställningar, objekt, ...etc. |
| BookSettings | `1048576` | Läs in inställningar för arbetsbok |
| Settings | `1114112` | Läs in inställningar för arbetsbok och arbetsblad |
| XmlMap | `2097152` | Läs in XmlMap |
| Structure | `4194304` | Läs in strukturen för arbetsboken |
| DocumentProperties | `8388608` | Läs in dokumentegenskaper |
| DefinedNames | `16777216` | Läs in definierade Namn-objekt |
| VBA | `33554432` | Ladda VBA-projekt |
| Style | `67108864` | Ladda stilar för cellformatering |
| Picture | `134217728` | Ladda bilder |
| OleObject | `268435456` | Ladda OleObjects |
| Revision | `536870912` | Ladda revisionsloggar |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadDataFilterOptionsDemo
    {
        public static void LoadDataFilterOptionsExample()
        {
            // Skapa en ny LoadOptions-instans
            LoadOptions loadOptions = new LoadOptions();

            // Skapa en anpassad LoadFilter-implementation
            loadOptions.LoadFilter = new CustomLoadFilter();

            // Läs in arbetsboken med de angivna inläsningsalternativen
            Workbook workbook = new Workbook("LoadDataFilterOptionsExample_original.xlsx", loadOptions);

            // Spara arbetsboken för att verifiera de laddade data
            workbook.Save("LoadDataFilterOptionsExample.xlsx");
        }

        // Anpassad LoadFilter-implementation
        private class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                // Tillämpa olika filteralternativ baserat på bladnamnet
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


