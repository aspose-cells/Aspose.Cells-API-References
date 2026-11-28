---
title: "WorkbookSettings.IsProtected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings property. Çalışma kitabının yapısının veya penceresinin korunup korunmadığını gösteren bir değer alır"
type: docs
url: /tr/net/aspose.cells/workbooksettings/isprotected/
---
## WorkbookSettings.IsProtected property

Çalışma kitabının yapısının veya penceresinin korunup korunmadığını gösteren bir değeri alır.

```csharp
public bool IsProtected { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;
            
            // Çalışma kitabının korunup korunmadığını kontrol et
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Çalışma kitabını bir şifreyle koru
            settings.Password = "password123";
            
            // Koruma durumunu doğrula
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Korunan çalışma kitabını kaydet
            workbook.Save("ProtectedWorkbook.xlsx", SaveFormat.Xlsx);
            
            // Korunan çalışma kitabını aç
            Workbook protectedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            
            // Yüklenen çalışma kitabının koruma durumunu kontrol et
            Console.WriteLine("Loaded workbook is protected: " + protectedWorkbook.Settings.IsProtected);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


