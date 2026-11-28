---
title: "GlobalizationSettings.ListSeparator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings özelliği. Fonksiyonun ... vb. liste parametreleri için ayırıcıyı alır"
type: docs
url: /tr/net/aspose.cells/globalizationsettings/listseparator/
---
## GlobalizationSettings.ListSeparator property

Liste, fonksiyon parametreleri, ... vb. için ayırıcıyı alır.

```csharp
public virtual char ListSeparator { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Özel küreselleştirme ayarlarıyla yeni bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özel ayarlarımıza ait mevcut ListSeparator değerini göster
            Console.WriteLine("Current ListSeparator value: " + workbook.Settings.GlobalizationSettings.ListSeparator);

            // Özel liste ayırıcıyı kullanarak formül oluşturun
            worksheet.Cells["A1"].Formula = "=CONCATENATE(\"Hello\"; \" World\")";
            worksheet.Cells["A2"].Formula = "=SUM(1;2;3)";

            // Özel ayırıcıyla formülleri hesaplayın
            workbook.CalculateFormula();

            // Hesaplama sonuçlarını göster
            Console.WriteLine("Concatenation result: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Sum result: " + worksheet.Cells["A2"].Value);

            // Özel liste ayırıcıyı kullanan formüllerle kaydedin
            workbook.Save("ListSeparatorDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ListSeparator => ';';
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


