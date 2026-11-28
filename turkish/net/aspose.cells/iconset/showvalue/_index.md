---
title: "IconSet.ShowValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IconSet özelliği. Bu simge setinin uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini belirten bayrağı alır veya ayarlar. Varsayılan değer true'tir."
type: docs
url: /tr/net/aspose.cells/iconset/showvalue/
---
## IconSet.ShowValue property

Bu ikon setinin uygulandığı hücrelerin değerlerini gösterip göstermediğini belirten bayrağı alın veya ayarlayın. Varsayılan değer true'dur.

```csharp
public bool ShowValue { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyShowValueDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);
            sheet.Cells["A5"].PutValue(50);

            // Simge seti koşullu biçimlendirmesi ekle
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            int index = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[index];

            // Simge seti özelliklerini ayarla
            condition.IconSet.Type = IconSetType.TrafficLights31;
            condition.IconSet.ShowValue = false; // This hides cell values and shows only icons
            condition.IconSet.Reverse = false;

            // Koşullu biçimlendirme için aralığı ayarla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            formatConditions.AddArea(area);

            // Çalışma kitabını kaydedin
            workbook.Save("IconSetShowValueDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon set conditional formatting (ShowValue = false).");
        }
    }
}
```

### Ayrıca Bakınız

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


