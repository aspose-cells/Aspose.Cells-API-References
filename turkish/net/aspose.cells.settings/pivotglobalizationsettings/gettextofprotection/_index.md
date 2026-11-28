---
title: "PivotGlobalizationSettings.GetTextOfProtection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. PivotTable'daki koruma adını alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotection/
---
## PivotGlobalizationSettings.GetTextOfProtection method

PivotTable'daki koruma adını alır.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetTextOfProtection()
```

### Dönüş Değeri

PivotTable'ın koruma adı

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotGlobalizationSettings.GetTextOfProtectedName(string) yöntemini kullanın. Bu özellik, Mart 2023'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectionDemo
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

            // Küreselleştirme ayarlarını oluşturun ve GetTextOfProtection yöntemini gösterin
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            Console.WriteLine("Protection Text: " + globalizationSettings.GetTextOfProtection());

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


