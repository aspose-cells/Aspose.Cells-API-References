---
title: "IconFilter.IconSetType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IconFilter özelliği. Bu filtre kriteri için kullanılan simge setini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/iconfilter/iconsettype/
---
## IconFilter.IconSetType property

Bu filtre ölçütü için kullanılan simge kümesini alır ve ayarlar.

```csharp
public IconSetType IconSetType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek verileri doldur
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Otomatik filtre oluştur
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;

            // Simge filtresini al
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;

            // Mevcut IconSetType'ı göster (varsayılan None'dır)
            Console.WriteLine("Current IconSetType: " + iconFilter.IconSetType);

            // 3 ok simge setine ayarla
            iconFilter.IconSetType = IconSetType.Arrows3;
            iconFilter.IconId = 1; // Show only middle arrow

            // Simgeleri görselleştirmek için koşullu biçimlendirme uygula
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.Arrows3;
            
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Trafik ışıkları simge setine değiştir
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 2; // Show only green light

            // Sonucu kaydet
            workbook.Save("PropertyIconSetTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [IconSetType](../../iconsettype/)
* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


