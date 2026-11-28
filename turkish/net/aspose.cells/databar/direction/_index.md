---
title: "DataBar.Direction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataBar özelliği. Veri çubuğunun görüntüleneceği yönü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/databar/direction/
---
## DataBar.Direction property

DataBar'ın görüntülendiği yönü alır veya ayarlar.

```csharp
public TextDirectionType Direction { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarPropertyDirectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Veri çubuklarını göstermek için örnek veri ekleyin
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;  // Values from 1 to 10 in column A
            }

            // Veri çubuğu koşullu biçimlendirmesi ekle
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection conditionalFormatting = conditionalFormattings[index];
            
            // Biçim koşulu için hücre alanını tanımlayın
            CellArea cellArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 9,
                EndColumn = 0
            };
            conditionalFormatting.AddArea(cellArea);

            // DataBar koşulunu ekleyin ve referansı alın
            int conditionIndex = conditionalFormatting.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditionalFormatting[conditionIndex];

            DataBar dataBar = condition.DataBar;

            // Mevcut Direction değerini göster
            Console.WriteLine("Initial DataBar Direction: " + dataBar.Direction);

            // Yönü RightToLeft olarak değiştirin ve gösterin
            dataBar.Direction = TextDirectionType.RightToLeft;

            // Daha iyi görselleştirme için ek yapılandırma
            dataBar.Color = System.Drawing.Color.LightGreen;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;

            // Etkisini göstermek için çalışma kitabını kaydedin
            workbook.Save("DataBarDirectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextDirectionType](../../textdirectiontype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


