---
title: "Enum MemorySetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.MemorySetting enum. Hücre veri modeli için bellek kullanım modları"
type: docs
url: /tr/net/aspose.cells/memorysetting/
---
## MemorySetting enumeration

Hücre veri modeli için bellek kullanım modları.

```csharp
public enum MemorySetting
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Normal | `0` | Hücre modeli için varsayılan mod. |
| MemoryPreference | `1` | Bellek performansı tercih edilir. |
| FileCache | `2` | Bellek performansı tercih edilir ve hücre verilerini tutmak için bellek yerine dosya kullanılır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MemorySettingDemo
    {
        public static void MemorySettingExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına erişin
            WorkbookSettings settings = workbook.Settings;

            // Bellek kullanım seçeneğini MemoryPreference olarak ayarlayın
            settings.MemorySetting = MemorySetting.MemoryPreference;

            // Bir çalışma sayfası oluşturun ve bazı veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);

            // Çalışma kitabını kaydedin
            workbook.Save("MemorySettingExample.xlsx");

            Console.WriteLine("Workbook saved with MemorySetting.MemoryPreference.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


