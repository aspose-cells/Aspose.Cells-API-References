---
title: "Font.IsSuperscript"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Yazı tipi özelliği. Yazı tipinin üst simge (superscript) olup olmadığını gösteren bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/font/issuperscript/
---
## Font.IsSuperscript property

Yazı tipinin üst simge olup olmadığını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IsSuperscript { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSuperscriptDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine metin ekle
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Normal Text Superscript Text");
            
            // Metnin bir kısmını üst simge (superscript) olarak biçimlendir
            FontSetting setting = cell.Characters(12, 11);
            setting.Font.IsSuperscript = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("FontIsSuperscriptDemo.xlsx");
            
            // Üst simge ayarını doğrulayın
            Console.WriteLine("IsSuperscript property: " + setting.Font.IsSuperscript);
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


