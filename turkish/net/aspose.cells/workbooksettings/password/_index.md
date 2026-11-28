---
title: "WorkbookSettings.Password"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma kitabı dosyası şifreleme parolasını temsil eder"
type: docs
url: /tr/net/aspose.cells/workbooksettings/password/
---
## WorkbookSettings.Password property

Workbook dosya şifreleme parolasını temsil eder.

```csharp
public string Password { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İlk çalışma sayfasına erişin ve bazı veriler ekleyin
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["C6"].PutValue("test encrypt.");
            
            // Çalışma kitabını korumak için parolayı ayarla
            wb.Settings.Password = "xixi";
            
            // Çalışma kitabını kaydedin
            wb.Save("output_with_password.ods");
            
            // Korunan çalışma kitabını açmak için parola ile yükleme seçenekleri oluştur
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "xixi";
            
            // Parola korumalı çalışma kitabını aç
            Workbook wbProtected = new Workbook("output_with_password.ods", loadOptions);
            
            // Verileri doğrula
            Console.WriteLine("Cell value: " + wbProtected.Worksheets[0].Cells["C6"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


