---
title: "Enum IconSetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.IconSetType-enum. Ikonsettyp för villkorsstyrd formatering. Tröskelvärdena för att utlösa de olika ikonerna inom ett set är konfigurerbara och ikonordningen är omvändningsbar"
type: docs
url: /sv/net/aspose.cells/iconsettype/
---
## IconSetType enumeration

Ikonuppsättningstyp för villkorsstyrd formatering. Tröskelvärdena för att utlösa de olika ikonerna inom en uppsättning är konfigurerbara, och ikonordningen kan vändas.

```csharp
public enum IconSetType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Arrows3 | `0` | 3-pilsikonset. |
| ArrowsGray3 | `1` | 3-gråa-pilsikonset. |
| Flags3 | `2` | 3-flaggaikonset. |
| Signs3 | `3` | 3-teckenikonset. |
| Symbols3 | `4` | 3-symbolikonset (cirkulerat). |
| Symbols32 | `5` | 3-symbolikonset (okringlat). |
| TrafficLights31 | `6` | 3 trafikljusikonset (utan ram). |
| TrafficLights32 | `7` | 3 trafikljusikonset med tjock svart kant. |
| Arrows4 | `8` | 4-pilsikonset. |
| ArrowsGray4 | `9` | 4-gråa-pilsikonset. |
| Rating4 | `10` | 4 betygsikonuppsättning. |
| RedToBlack4 | `11` | 4 'röd till svart' ikonuppsättning. |
| TrafficLights4 | `12` | 4 trafikljusikonuppsättning. |
| Arrows5 | `13` | 5 pilikonuppsättning. |
| ArrowsGray5 | `14` | 5 gråa pilikonuppsättning. |
| Quarters5 | `15` | 5 kvartalsikonuppsättning. |
| Rating5 | `16` | 5 betygsikonuppsättning. |
| Stars3 | `17` | 3 stjärnuppsättning |
| Boxes5 | `18` | 5 boxuppsättning |
| Triangles3 | `19` | 3 triangeluppsättning |
| None | `20` | Ingen |
| CustomSet | `21` | CustomSet. Detta element är skrivskyddat. |
| Smilies3 | `22` | 3 smileys. Endast för .ods. |
| ColorSmilies3 | `23` | 3 färgade smileys. Endast för .ods. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIconSetTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Ange exempelvärden
            cells["A1"].PutValue(1);
            cells["A2"].PutValue("#DIV/0!");
            cells["A3"].PutValue(3);

            // Lägg till villkorsstyrd formatering med ikonuppsättning
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
            
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
            fc.IconSet.Type = IconSetType.TrafficLights31;

            // Hämta och visa resultat
            ConditionalFormattingResult res1 = cells["A1"].GetConditionalFormattingResult();
            Console.WriteLine($"A1 Icon Type: {res1.ConditionalFormattingIcon.Type}, Index: {res1.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res3 = cells["A3"].GetConditionalFormattingResult();
            Console.WriteLine($"A3 Icon Type: {res3.ConditionalFormattingIcon.Type}, Index: {res3.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res2 = cells["A2"].GetConditionalFormattingResult();
            Console.WriteLine($"A2 has formatting: {res2 != null && res2.ConditionalFormattingIcon != null}");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


