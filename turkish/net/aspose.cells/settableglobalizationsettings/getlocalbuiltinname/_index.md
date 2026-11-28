---
title: "SettableGlobalizationSettings.GetLocalBuiltInName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Verilen standart metne göre yerel bağımlı yerleşik Name metnini alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/getlocalbuiltinname/
---
## SettableGlobalizationSettings.GetLocalBuiltInName method

Verilen standart metne göre yerel ayara bağlı yerleşik Name metnini alır.

```csharp
public override string GetLocalBuiltInName(string standardName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| standardName | String | Yerleşik Name'in Standart (en-US yereli) metni. |

### Dönüş Değeri

Yerel bağımlı metin. Yerel, bu ayarların kullanıldığı Workbook tarafından belirtilmiştir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SettableGlobalizationSettings örneği oluştur
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // GetLocalBuiltInName yöntemini standart bir yerleşik adla çağır
                string standardName = "SUM";
                string localName = globalizationSettings.GetLocalBuiltInName(standardName);

                // Sonucu göster
                Console.WriteLine($"Standard name: {standardName}, Local name: {localName}");

                // Standart yerleşik ad için özel bir yerel ad ayarla
                globalizationSettings.SetLocalBuiltInName(standardName, "CustomSum", true);

                // Ayarladıktan sonra yerel adı tekrar al
                localName = globalizationSettings.GetLocalBuiltInName(standardName);
                Console.WriteLine($"After setting - Standard name: {standardName}, Local name: {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("MethodGetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


