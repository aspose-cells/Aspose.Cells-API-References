---
title: "FontSetting.FontSetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSetting yapıcı."
type: docs
url: /tr/net/aspose.cells/fontsetting/fontsetting/
---
## FontSetting constructor

```csharp
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | Int32 |  |
| uzunluk | Int32 |  |
| sayfalar | WorksheetCollection |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingMethodCtorWithInt32Int32WorksheetCollectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücreye örnek metin ekle
            worksheet.Cells["A1"].PutValue("Hello World");
            
            // Tüm çalışma sayfalarında ilk 5 karakter (0-4) için yazı tipi ayarı oluşturun
            FontSetting fontSetting = new FontSetting(0, 5, workbook.Worksheets);
            
            // Biçimlendirmeyi uygula
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Size = 14;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


