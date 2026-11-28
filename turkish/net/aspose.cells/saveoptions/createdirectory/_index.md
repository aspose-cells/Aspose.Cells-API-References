---
title: "SaveOptions.CreateDirectory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SaveOptions özelliği. True ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur"
type: docs
url: /tr/net/aspose.cells/saveoptions/createdirectory/
---
## SaveOptions.CreateDirectory property

Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.

```csharp
public bool CreateDirectory { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCreateDirectoryDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek veri ekleyin.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // CreateDirectory etkinleştirilmiş şekilde kaydetme seçeneklerini ayarlayın
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.CreateDirectory = true;

            // Çalışma kitabını yeni bir dizine kaydedin (otomatik olarak oluşturulacaktır)
            string outputPath = "OutputDirectory/example.xls";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved successfully with directory creation.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


