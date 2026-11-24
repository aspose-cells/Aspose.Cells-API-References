---
title: "Aufzählung IconSetType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.IconSetType enum. Symbolsatztyp für die bedingte Formatierung. Die Schwellenwerte zum Auslösen der verschiedenen Symbole innerhalb eines Satzes sind konfigurierbar und die Symbolreihenfolge ist umkehrbar."
type: docs
url: /de/net/aspose.cells/iconsettype/
---
## IconSetType enumeration

Icon-Set-Typ für bedingte Formatierung. Die Schwellenwerte zum Auslösen der verschiedenen Symbole innerhalb eines Sets sind konfigurierbar, und die Symbolreihenfolge ist umkehrbar.

```csharp
public enum IconSetType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Arrows3 | `0` | 3‑Pfeile‑Symbolsatz. |
| ArrowsGray3 | `1` | 3 graue Pfeile Symbolsatz. |
| Flags3 | `2` | 3 Flaggen Symbolsatz. |
| Signs3 | `3` | 3 Schilder Symbolsatz. |
| Symbols3 | `4` | 3 Symbole Symbolsatz (eingekreist). |
| Symbols32 | `5` | 3 Symbole Symbolsatz (nicht eingekreist). |
| TrafficLights31 | `6` | 3 Ampeln Symbolsatz (ohne Rand). |
| TrafficLights32 | `7` | 3 Ampeln Symbolsatz mit dickem schwarzem Rand. |
| Arrows4 | `8` | 4 Pfeile Symbolsatz. |
| ArrowsGray4 | `9` | 4 graue Pfeile Symbolsatz. |
| Rating4 | `10` | 4 Bewertungs‑Symbolsatz. |
| RedToBlack4 | `11` | 4 'rot zu schwarz' Symbolsatz. |
| TrafficLights4 | `12` | 4 Ampeln Symbolsatz. |
| Arrows5 | `13` | 5 Pfeile Symbolsatz. |
| ArrowsGray5 | `14` | 5 graue Pfeile Symbolsatz. |
| Quarters5 | `15` | 5 Viertel Symbolsatz. |
| Rating5 | `16` | 5 Bewertungs‑Symbolsatz. |
| Stars3 | `17` | 3‑Sterne‑Satz |
| Boxes5 | `18` | 5‑Kästen‑Satz |
| Triangles3 | `19` | 3‑Dreiecke‑Satz |
| None | `20` | Keine |
| CustomSet | `21` | CustomSet. Dieses Element ist schreibgeschützt. |
| Smilies3 | `22` | 3 Smilies. Nur für .ods. |
| ColorSmilies3 | `23` | 3 farbige Smilies. Nur für .ods. |

### Beispiele

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

            // Beispielwerte festlegen
            cells["A1"].PutValue(1);
            cells["A2"].PutValue("#DIV/0!");
            cells["A3"].PutValue(3);

            // Bedingte Formatierung mit Symbolsatz hinzufügen
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
            
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
            fc.IconSet.Type = IconSetType.TrafficLights31;

            // Ergebnisse abrufen und anzeigen
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

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


