---
title: "WorkbookSettings.ProtectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma kitabının koruma türünü alır"
type: docs
url: /tr/net/aspose.cells/workbooksettings/protectiontype/
---
## WorkbookSettings.ProtectionType property

Workbook'un koruma türünü alır.

```csharp
public ProtectionType ProtectionType { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyProtectionTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabını Windows koruma türüyle koru
            workbook.Protect(ProtectionType.Windows, "password123");
            
            // ProtectionType özelliğini göster
            Console.WriteLine("Workbook protection type: " + workbook.Settings.ProtectionType);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ProtectedWorkbook.xlsx");
            
            // Kaydedilmiş çalışma kitabını yükleyerek koruma türünün devam ettiğini doğrula
            Workbook loadedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            Console.WriteLine("Loaded workbook protection type: " + loadedWorkbook.Settings.ProtectionType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [ProtectionType](../../protectiontype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


