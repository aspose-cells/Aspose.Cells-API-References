---
title: "WorkbookSettings.Shared"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma kitabının paylaşılıp paylaşılmadığını gösteren bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/shared/
---
## WorkbookSettings.Shared property

Workbook'un paylaşılıp paylaşılmadığını belirten bir değeri alır veya ayarlar.

```csharp
public bool Shared { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySharedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook book = new Workbook();
            
            // Shared özelliğini true olarak ayarla
            book.Settings.Shared = true;
            
            // Çalışma kitabını kaydedin
            string outputPath = "output_shared.xlsx";
            book.Save(outputPath);
            
            // Shared özelliğini doğrulamak için kaydedilmiş çalışma kitabını yükle
            Workbook loadedBook = new Workbook(outputPath);
            Console.WriteLine("Shared property value: " + loadedBook.Settings.Shared);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


