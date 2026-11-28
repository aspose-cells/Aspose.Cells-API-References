---
title: "PivotGlobalizationSettings.GetTextOfAll"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. PivotTable'da Tüm etiketi metnini alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofall/
---
## PivotGlobalizationSettings.GetTextOfAll method

PivotTable'daki "(All)" etiketinin metnini alır.

```csharp
public virtual string GetTextOfAll()
```

### Dönüş Değeri

"(All)" etiketinin metni

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfAllDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Küreselleştirme ayarlarını oluştur ve kullan
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // GetTextOfAll yöntemini göster
            Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());

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


