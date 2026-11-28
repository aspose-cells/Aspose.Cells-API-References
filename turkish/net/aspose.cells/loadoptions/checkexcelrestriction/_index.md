---
title: "LoadOptions.CheckExcelRestriction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarını kontrol edip kontrol etmeyeceği. Örneğin Excel, 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValuestring ile 32K'dan uzun bir değer girdiğinizde bu özellik true ise bir Exception alırsınız. Bu özellik false ise girdiğiniz dize değerini hücre değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak Excel dosya formatı için geçersiz olan böyle bir değer ayarladıysanız, çalışma kitabını daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar ortaya çıkabilir."
type: docs
url: /tr/net/aspose.cells/loadoptions/checkexcelrestriction/
---
## LoadOptions.CheckExcelRestriction property

Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Excel kısıtlama denetimini devre dışı bırak
            workbook.Settings.CheckExcelRestriction = false;

            // İlk çalışma sayfasına ve hücrelere erişin.
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Excel'in normal sınırından (32767 karakter) daha uzun bir dize oluştur
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Uzun dizeyi A1 hücresine koyun.
            cells["A1"].PutValue(longString);
            
            // Kısıtlama denetimi devre dışı bırakılarak kaydet
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;
            workbook.Save("output.xlsx", saveOptions);
            
            // Kısıtlama denetimi devre dışı bırakılarak yükle
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output.xlsx", loadOptions);
            
            // Uzun dizeyin korunduğunu doğrulayın.
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("String length: " + loadedValue.Length);
            Console.WriteLine("String matches: " + loadedValue.Equals(longString));
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


