---
title: "WorkbookSettings.SignificantDigitsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Bu çalışma kitabında sayısal değerleri çıkarmak için anlamlı basamak türünü alır ve ayarlar. Varsayılan değer SignificantDigitsType'dir."
type: docs
url: /tr/net/aspose.cells/workbooksettings/significantdigitstype/
---
## WorkbookSettings.SignificantDigitsType property

Bu çalışma kitabında sayısal değerleri çıkarmak için anlamlı basamak türünü alır ve ayarlar. Varsayılan değer [`SignificantDigitsType`](../../cellshelper/significantdigitstype/).

```csharp
public SignificantDigitsType SignificantDigitsType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;

            // Geçerli SignificantDigitsType değerini göster
            Console.WriteLine("Current SignificantDigitsType: " + settings.SignificantDigitsType);

            // Farklı SignificantDigitsType değerlerini ayarlamayı göster
            settings.SignificantDigitsType = SignificantDigitsType.Digits15;
            Console.WriteLine("After setting to Digits15: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.G17;
            Console.WriteLine("After setting to G17: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.Rounding17;
            Console.WriteLine("After setting to Rounding17: " + settings.SignificantDigitsType);

            // Etkiyi göstermek için bazı sayısal veriler ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(123.4567890123456789);
            worksheet.Cells["A2"].PutValue(9876543210.123456789);

            // Çalışma kitabını kaydedin
            workbook.Save("SignificantDigitsTypeDemo.xlsx");
            Console.WriteLine("Workbook saved with SignificantDigitsType settings.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


