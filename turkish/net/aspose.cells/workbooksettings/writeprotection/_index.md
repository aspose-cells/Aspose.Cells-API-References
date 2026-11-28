---
title: "WorkbookSettings.WriteProtection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma kitabı yazma koruma seçeneklerine erişim sağlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

Çalışma kitabının yazma koruma seçeneklerine erişim sağlar.

```csharp
public WriteProtection WriteProtection { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWriteProtectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yazma koruma özelliklerini ayarla
            workbook.Settings.WriteProtection.Password = "test123";
            workbook.Settings.WriteProtection.Author = "John Doe";
            workbook.Settings.WriteProtection.RecommendReadOnly = true;

            // Çalışma kitabını kaydedin
            string outputPath = "WriteProtectionDemo.xlsx";
            workbook.Save(outputPath);

            // Kaydedilmiş çalışma kitabını yükleyerek özellikleri doğrulayın
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Yazma koruma özelliklerini çıktı olarak göster
            Console.WriteLine("Author: " + loadedWorkbook.Settings.WriteProtection.Author);
            Console.WriteLine("ReadOnly Recommended: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
        }
    }
}
```

### Ayrıca Bakınız

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


