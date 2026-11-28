---
title: "LoadOptions.SetPaperSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions yöntemi. Varsayılan yazıcı ayarlarından varsayılan baskı kağıt boyutunu ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/setpapersize/
---
## LoadOptions.SetPaperSize method

Varsayılan yazıcının ayarlarından varsayılan baskı kağıdı boyutunu ayarlar.

```csharp
public void SetPaperSize(PaperSizeType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | PaperSizeType | Varsayılan kağıt boyutu. |

### Açıklamalar

Kağıt boyutu ile ilgili bir ayar yoksa, MS Excel varsayılan yazıcı ayarını kullanır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsMethodSetPaperSizeWithPaperSizeTypeDemo
    {
        public static void Run()
        {
            // Yükleme seçeneklerini oluştur ve kağıt boyutunu A5 olarak ayarla
            LoadOptions options = new LoadOptions();
            options.SetPaperSize(PaperSizeType.PaperA5);

            // Belirtilen seçeneklerle çalışma kitabını yükle
            Workbook workbook = new Workbook("example.xlsx", options);
            
            // Kağıt boyutunun doğru ayarlandığını doğrula
            Console.WriteLine("Paper size of first worksheet: " + workbook.Worksheets[0].PageSetup.PaperSize);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


