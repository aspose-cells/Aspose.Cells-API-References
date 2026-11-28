---
title: "SettableGlobalizationSettings.ListSeparator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings özelliği. Fonksiyonun ...etc liste parametreleri için ayırıcıyı alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/listseparator/
---
## SettableGlobalizationSettings.ListSeparator property

Liste, fonksiyon parametreleri, ... vb. için ayırıcıyı alır.

```csharp
public override char ListSeparator { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // SettableGlobalizationSettings örneği oluştur
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Mevcut ListSeparator değerini göster (çoğu yerel ayarda varsayılan virgüldür)
            Console.WriteLine("Current ListSeparator value: " + settings.ListSeparator);
            
            // Yeni bir ListSeparator değeri ayarla (ör. noktalı virgül)
            settings.SetListSeparator(';');
            
            // Ayarları çalışma kitabına uygula
            workbook.Settings.GlobalizationSettings = settings;
            
            // Formül ayrıştırmada ListSeparator etkisini göster
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue("Data");
            
            // Liste ayırıcıyı kullanan bir formül oluştur
            worksheet.Cells["A3"].Formula = "=CONCATENATE(A1,A2)";
            
            // Formül, ayrıştırıldığında özel liste ayırıcıyı kullanacak
            Console.WriteLine("Formula with custom separator: " + worksheet.Cells["A3"].Formula);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PropertyListSeparatorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


