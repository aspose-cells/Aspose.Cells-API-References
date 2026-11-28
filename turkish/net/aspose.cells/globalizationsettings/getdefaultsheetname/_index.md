---
title: "GlobalizationSettings.GetDefaultSheetName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "GlobalizationSettings yöntemi. Çalışma sayfasını otomatik eklemek için varsayılan sayfa adını alır. Varsayılan \"Sheet\"tir."
type: docs
url: /tr/net/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings.GetDefaultSheetName method

Çalışma sayfası otomatik olarak eklenirken varsayılan sayfa adını alır. Varsayılan "Sheet".

```csharp
public virtual string GetDefaultSheetName()
```

### Dönüş Değeri

çalışma sayfasını otomatik eklemek için varsayılan sayfa adı

### Açıklamalar

Otomatik eklenen (örneğin [`Add`](../../worksheetcollection/add/) ile) sayfanın adı belirtilen ad artı sıra numarası olacaktır. Örneğin, Almanya kullanıcısı sayfa adının "Sheet2" yerine "Tabellenblatt2" olmasını isteyebilir. Bu durumda kullanıcı bu yöntemi "Tabellenblatt" döndürecek şekilde uygulayabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetDefaultSheetNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Özel küreselleştirme ayarlarını ayarla
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Özel globalizasyon ayarlarından varsayılan sayfa adını al
                string defaultSheetName = workbook.Settings.GlobalizationSettings.GetDefaultSheetName();
                Console.WriteLine($"Default sheet name retrieved: {defaultSheetName}");

                // Özel varsayılan üzerine adlandırmayı göstermek için yeni bir çalışma sayfası ekle
                int sheetIndex = workbook.Worksheets.Add();
                Worksheet newWorksheet = workbook.Worksheets[sheetIndex];
                Console.WriteLine($"New worksheet name after method call: {newWorksheet.Name}");

                Console.WriteLine("GetDefaultSheetName method demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDefaultSheetName method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("MethodGetDefaultSheetNameDemo.xlsx");
        }
    }

    // Özel globalizasyon ayarları uygulaması
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDefaultSheetName()
        {
            return "CustomSheet"; // Custom default sheet name
        }
    }
}
```

### Ayrıca Bakınız

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


