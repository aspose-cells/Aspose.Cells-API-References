---
title: "WorkbookSettings.PaperSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Varsayılan yazdırma kağıt boyutunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/papersize/
---
## WorkbookSettings.PaperSize property

Varsayılan yazdırma kağıt boyutunu alır ve ayarlar.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Açıklamalar

Kağıt boyutu ile ilgili bir ayar yoksa, MS Excel varsayılan yazıcı ayarını kullanır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Kağıt boyutunu A5 olarak ayarla
            workbook.Settings.PaperSize = PaperSizeType.PaperA5;
            
            // Kağıt boyutunun ilk çalışma sayfasında doğru ayarlandığını doğrula
            Console.WriteLine("Paper size: " + workbook.Worksheets[0].PageSetup.PaperSize);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PaperSizeType](../../papersizetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


