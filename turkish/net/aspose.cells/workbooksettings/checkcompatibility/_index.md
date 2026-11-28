---
title: "WorkbookSettings.CheckCompatibility"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma kitabı kaydedilirken daha eski sürümlerle uyumluluğun kontrol edilip edilmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/checkcompatibility/
---
## WorkbookSettings.CheckCompatibility property

Çalışma kitabı kaydedilirken önceki sürümlerle uyumluluğun kontrol edilip edilmediğini gösterir.

```csharp
public bool CheckCompatibility { get; set; }
```

### Açıklamalar

Varsayılan değer true'dur. Yalnızca Excel97-2003 xls veya xlt dosyaları için.

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckCompatibilityDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // CheckCompatibility'ı true olarak ayarla ve kaydet
            workbook.Settings.CheckCompatibility = true;
            workbook.Save("CheckCompatibilityDemo_true.xlsx");
            
            // Yeniden yükle ve doğrula
            workbook = new Workbook("CheckCompatibilityDemo_true.xlsx");
            Console.WriteLine("CheckCompatibility (true): " + workbook.Settings.CheckCompatibility);
            
            // CheckCompatibility'ı false olarak ayarla ve kaydet
            workbook.Settings.CheckCompatibility = false;
            workbook.Save("CheckCompatibilityDemo_false.xlsx");
            
            // Yeniden yükle ve doğrula
            workbook = new Workbook("CheckCompatibilityDemo_false.xlsx");
            Console.WriteLine("CheckCompatibility (false): " + workbook.Settings.CheckCompatibility);
            
            // Renk işlemlerini göster
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color customColor = workbook.GetMatchingColor(Color.FromArgb(255, 123, 123, 123));
            Console.WriteLine("Matching color R value: " + customColor.R);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


