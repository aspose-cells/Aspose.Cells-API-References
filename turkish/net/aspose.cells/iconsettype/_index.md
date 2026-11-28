---
title: "Enum IconSetType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.IconSetType enum. Koşullu biçimlendirme için simge seti türü. Bir set içinde farklı simgelerin tetiklenmesi için eşik değerleri yapılandırılabilir ve simge sırası tersine çevrilebilir."
type: docs
url: /tr/net/aspose.cells/iconsettype/
---
## IconSetType enumeration

Koşullu biçimlendirme için simge seti türü. Bir set içindeki farklı simgelerin tetiklenmesi için eşik değerleri yapılandırılabilir ve simge sırası tersine çevrilebilir.

```csharp
public enum IconSetType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Arrows3 | `0` | 3 ok simge seti. |
| ArrowsGray3 | `1` | 3 gri ok simge seti. |
| Flags3 | `2` | 3 bayrak simge seti. |
| Signs3 | `3` | 3 işaret simge seti. |
| Symbols3 | `4` | 3 sembol simge seti (dairesel). |
| Symbols32 | `5` | 3 sembol simge seti (dairesiz). |
| TrafficLights31 | `6` | 3 trafik ışığı simge seti (kenarsız). |
| TrafficLights32 | `7` | Kalın siyah kenarlı 3 trafik ışığı simge seti. |
| Arrows4 | `8` | 4 ok simge seti. |
| ArrowsGray4 | `9` | 4 gri ok simge seti. |
| Rating4 | `10` | 4 derecelendirme simge seti. |
| RedToBlack4 | `11` | 4 'kırmızıdan siyaha' simge seti. |
| TrafficLights4 | `12` | 4 trafik ışığı simge seti. |
| Arrows5 | `13` | 5 ok simgesi seti. |
| ArrowsGray5 | `14` | 5 gri ok simgesi seti. |
| Quarters5 | `15` | 5 çeyrek simgesi seti. |
| Rating5 | `16` | 5 puanlama simgesi seti. |
| Stars3 | `17` | 3 yıldız seti |
| Boxes5 | `18` | 5 kutu seti |
| Triangles3 | `19` | 3 üçgen seti |
| None | `20` | Yok |
| CustomSet | `21` | CustomSet. Bu öğe yalnızca okunabilir. |
| Smilies3 | `22` | 3 gülümseme. Yalnızca .ods için. |
| ColorSmilies3 | `23` | 3 renkli gülümseme. Yalnızca .ods için. |

### Örnekler

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

            // Örnek değerleri ayarla
            cells["A1"].PutValue(1);
            cells["A2"].PutValue("#DIV/0!");
            cells["A3"].PutValue(3);

            // Simge seti ile koşullu biçimlendirme ekle
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
            
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
            fc.IconSet.Type = IconSetType.TrafficLights31;

            // Sonuçları al ve göster
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

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


