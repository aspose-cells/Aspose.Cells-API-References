---
title: "IconSet.IsCustom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IconSet özelliği. Simge setinin özelleştirilmiş olup olmadığını gösterir. Varsayılan değer false'dur."
type: docs
url: /tr/net/aspose.cells/iconset/iscustom/
---
## IconSet.IsCustom property

İkon setinin özelleştirilmiş olup olmadığını gösterir. Varsayılan değer false'tur.

```csharp
public bool IsCustom { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyIsCustomDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Özel simge seti ile koşullu biçimlendirme ekleyin
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Koşullu biçimlendirme için aralığı ayarla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 9;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Simge seti koşulu ekle
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // Simge seti türünü ayarlayın (geçerli IconSetType kullanarak)
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // IsCustom özelliğini doğrulayın (yalnızca okunur)
            Console.WriteLine("Is IconSet custom? " + condition.IconSet.IsCustom);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


