---
title: "SaveOptions.WarningCallback"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SaveOptions özelliği. Uyarı geri aramasını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/saveoptions/warningcallback/
---
## SaveOptions.WarningCallback property

Uyarı geri çağrısını alır veya ayarlar.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data");

            // Kaydetme seçeneklerini oluşturun
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Özel uyarı geri aramasını ayarla
            saveOptions.WarningCallback = new CustomWarningCallback();

            // Bu, HTML formatında desteklenmeyen bir özellik hakkında bir uyarı oluşturacaktır
            worksheet.PageSetup.PrintTitleRows = "$1:$1";

            // Uyarı oluşturabilecek seçeneklerle kaydet
            workbook.Save("WarningCallbackDemo.html", saveOptions);
        }
    }

    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Uyarıyı işle - bu durumda sadece göster
            Console.WriteLine($"Warning: {warningInfo.Description}");
            Console.WriteLine($"Warning type: {warningInfo.WarningType}");
        }
    }
}
```

### Ayrıca Bakınız

* interface [IWarningCallback](../../iwarningcallback/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


