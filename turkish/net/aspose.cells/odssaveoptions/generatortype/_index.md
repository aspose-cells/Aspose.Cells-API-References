---
title: "OdsSaveOptions.GeneratorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsSaveOptions özelliği. ODS dosyasının oluşturucusunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/odssaveoptions/generatortype/
---
## OdsSaveOptions.GeneratorType property

ODS dosyasının oluşturucusunu alır ve ayarlar.

```csharp
public OdsGeneratorType GeneratorType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyGeneratorTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // ODS kaydetme seçeneklerini oluştur ve yapılandır
            OdsSaveOptions saveOptions = new OdsSaveOptions
            {
                GeneratorType = OdsGeneratorType.LibreOffice,
                IsStrictSchema11 = true
            };

            // Çalışma kitabını belirtilen seçeneklerle kaydet
            workbook.Save("OdsSaveOptions_GeneratorTypeDemo.ods", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [OdsGeneratorType](../../../aspose.cells.ods/odsgeneratortype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


