---
title: "Enum TextCrossType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TextCrossType enum. Metin genişliği hücre genişliğinden büyük olduğunda metin görüntüleme türünü belirtir."
type: docs
url: /tr/net/aspose.cells/textcrosstype/
---
## TextCrossType enumeration

Metin genişliği hücre genişliğinden büyük olduğunda metin görüntüleme tiplerini listeler.

```csharp
public enum TextCrossType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `1` | Metni Microsoft Excel'de olduğu gibi göster. |
| CrossKeep | `2` | Metni diğer hücrelerin üzerinden geçerek ve kesişen hücrelerin metnini koruyarak tüm metni göster. |
| CrossOverride | `3` | Diğer hücreleri geçerek tüm metni göster ve kesilen hücrelerin metnini geçersiz kıl. |
| StrictInCell | `4` | Metni yalnızca hücrenin genişliği içinde göster. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassTextCrossTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Taşma yapabilecek bir hücreye örnek metin ayarla
            worksheet.Cells["A1"].PutValue("This is a long text that might overflow the cell");
            
            // Görüntü veya yazdırma seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Farklı TextCrossType ayarlarını göster
            options.TextCrossType = TextCrossType.Default;
            SaveToImage(workbook, options, "TextCrossType_Default.png");
            
            options.TextCrossType = TextCrossType.CrossKeep;
            SaveToImage(workbook, options, "TextCrossType_CrossKeep.png");
            
            options.TextCrossType = TextCrossType.CrossOverride;
            SaveToImage(workbook, options, "TextCrossType_CrossOverride.png");
            
            options.TextCrossType = TextCrossType.StrictInCell;
            SaveToImage(workbook, options, "TextCrossType_StrictInCell.png");
        }
        
        private static void SaveToImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


