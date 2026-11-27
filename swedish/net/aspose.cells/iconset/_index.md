---
title: "Klass IconSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.IconSet klass. Beskriv IconSet-regeln för villkorsstyrd formatering. Denna regel för villkorsstyrd formatering tillämpar ikoner på celler enligt deras värden."
type: docs
url: /sv/net/aspose.cells/iconset/
---
## IconSet class

Beskriv regeln för IconSet‑villkorsstyrd formatering. Denna villkorsstyrda formateringsregel tillämpar ikoner på celler enligt deras värden.

```csharp
public class IconSet
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CfIcons](../../aspose.cells/iconset/cficons/) { get; } | Hämta den[`ConditionalFormattingIcon`](../conditionalformattingicon/) från samlingen |
| [Cfvos](../../aspose.cells/iconset/cfvos/) { get; } | Hämta CFValueObjects-instansen. |
| [IsCustom](../../aspose.cells/iconset/iscustom/) { get; } | Indikerar om ikonuppsättningen är anpassad. Standardvärdet är falskt. |
| [Reverse](../../aspose.cells/iconset/reverse/) { get; set; } | Hämta eller ange flaggan som indikerar om standardordningen för ikonerna i denna ikonuppsättning ska vändas. Standardvärdet är falskt. |
| [ShowValue](../../aspose.cells/iconset/showvalue/) { get; set; } | Hämta eller ange flaggan som indikerar om värdena i de celler som denna ikonuppsättning tillämpas på ska visas. Standardvärdet är sant. |
| [Type](../../aspose.cells/iconset/type/) { get; set; } | Hämta eller ange ikonutgångstypen som ska visas. Att ange typen kommer automatiskt att kontrollera om det aktuella antalet Cfods stämmer överens med den nya typen. Om det inte stämmer, kommer gamla Cfods att rensas och standard‑Cfods att läggas till. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetDemo
    {
        public static void IconSetExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägger till en tom villkorlig formatering
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Ställer in området för den villkorliga formateringen
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Lägger till villkor
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // Hämta ikonuppsättning
            IconSet iconSet = cond.IconSet;

            // Ange ikontyp
            iconSet.Type = IconSetType.Arrows3;

            // Ange ytterligare egenskaper
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Sätt cellvärden
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Sparar Excel-filen
            workbook.Save("IconSetExample.xlsx");
            workbook.Save("IconSetExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


