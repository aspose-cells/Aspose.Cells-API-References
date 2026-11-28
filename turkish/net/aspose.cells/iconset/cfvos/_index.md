---
title: "IconSet.Cfvos"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IconSet özelliği. CFValueObjects örneğini al"
type: docs
url: /tr/net/aspose.cells/iconset/cfvos/
---
## IconSet.Cfvos property

CFValueObjects örneğini alın.

```csharp
public ConditionalFormattingValueCollection Cfvos { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetPropertyCfvosDemo
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

            try
            {
                // Koşullu biçimlendirme ekle
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

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

                // Simge seti türünü ayarla
                condition.IconSet.Type = IconSetType.TrafficLights31;

                // Cfvos özelliğine erişin (yalnızca okunur)
                ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

                // Cfvos koleksiyonu hakkında bilgi gösterin
                Console.WriteLine("Number of CFValueObjects in the collection: " + cfvos.Count);

                // Koleksiyonun içinde yineleyin ve her değeri gösterin
                for (int i = 0; i < cfvos.Count; i++)
                {
                    ConditionalFormattingValue cfValue = cfvos[i];
                    Console.WriteLine($"CFValue {i + 1}: Type = {cfValue.Type}, Value = {cfValue.Value}");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("IconSetCfvosDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon set conditional formatting.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


