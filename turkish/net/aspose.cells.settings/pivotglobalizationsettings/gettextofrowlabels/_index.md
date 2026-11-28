---
title: "PivotGlobalizationSettings.GetTextOfRowLabels"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. PivotTable'da Satır Etiketleri etiketinin metnini alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/
---
## PivotGlobalizationSettings.GetTextOfRowLabels method

PivotTable'daki "Row Labels" etiketinin metnini alır.

```csharp
public virtual string GetTextOfRowLabels()
```

### Dönüş Değeri

Satır etiketlerinin metni

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B3"].PutValue(200);

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Küreselleştirme ayarlarını oluştur ve kullan
            PivotGlobalizationSettings settings = new PivotGlobalizationSettings();
            
            // GetTextOfRowLabels yöntemini göster
            Console.WriteLine("Row Labels Text: " + settings.GetTextOfRowLabels());

            // Çalışma kitabını kaydedin
            workbook.Save("PivotGlobalizationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


