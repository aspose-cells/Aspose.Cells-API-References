---
title: "WorkbookSettings.UpdateLinksType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma kitabı açıldığında dış bağlantıların nasıl güncelleneceğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/updatelinkstype/
---
## WorkbookSettings.UpdateLinksType property

Çalışma kitabı açıldığında dış bağlantıların nasıl güncelleneceğini alır ve ayarlar.

```csharp
public UpdateLinksType UpdateLinksType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyUpdateLinksTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // UpdateLinksType'ı Never olarak ayarlayın
            workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Ayarı doğrulamak için kaydedilmiş çalışma kitabını yükle
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // UpdateLinksType değerini çıktı olarak verin
            Console.WriteLine("UpdateLinksType: " + loadedWorkbook.Settings.UpdateLinksType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [UpdateLinksType](../../updatelinkstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


