---
title: "SaveOptions.CheckExcelRestriction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SaveOptions özelliği. Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmeyeceği. Örneğin Excel, 32K'dan uzun bir dize değerinin girilmesine izin vermez. 32K'dan uzun bir değer girerseniz kesilir."
type: docs
url: /tr/net/aspose.cells/saveoptions/checkexcelrestriction/
---
## SaveOptions.CheckExcelRestriction property

Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmeyeceği. Örneğin, Excel 32K'dan uzun metin değerlerinin girilmesine izin vermez. 32K'dan uzun bir değer girerseniz, kesilir.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Excel kısıtlama kontrolünü devre dışı bırakın.
            workbook.Settings.CheckExcelRestriction = false;

            // İlk çalışma sayfasına ve hücrelere erişin.
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Excel'in normal sınırından daha uzun bir dize oluşturun.
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Uzun dizeyi A1 hücresine koyun.
            cells["A1"].PutValue(longString);

            // Kısıtlamaları atlamak için kaydetme seçeneklerini yapılandırın.
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;

            // Çalışma kitabını kaydedin
            workbook.Save("output_without_restrictions.xlsx", saveOptions);

            // Kısıtlamalar devre dışı bırakılmış şekilde kaydedilen dosyayı yükleyin.
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output_without_restrictions.xlsx", loadOptions);

            // Uzun dizeyin korunduğunu doğrulayın.
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("Loaded string length: " + loadedValue.Length);
            Console.WriteLine("First 50 chars: " + loadedValue.Substring(0, 50));
            Console.WriteLine("Last 50 chars: " + loadedValue.Substring(loadedValue.Length - 50));
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


