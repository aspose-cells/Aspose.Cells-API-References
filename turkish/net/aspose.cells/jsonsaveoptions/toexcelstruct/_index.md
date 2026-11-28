---
title: "JsonSaveOptions.ToExcelStruct"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonSaveOptions özelliği. Excel dosyasının json yapısına dönüştürülüp dönüştürülmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/jsonsaveoptions/toexcelstruct/
---
## JsonSaveOptions.ToExcelStruct property

Excel dosyasının JSON yapısına dönüştürülüp dönüştürülmeyeceğini gösterir

```csharp
public bool ToExcelStruct { get; set; }
```

### Açıklamalar

Yalnızca aralığı JSON'a dönüştürmek için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyToExcelStructDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Dışa aktarmak için bir aralık oluştur
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

            // JSON kaydetme seçeneklerini ToExcelStruct ile yapılandır
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;

            // Aralığı JSON'a dışa aktar
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### Ayrıca Bakınız

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


