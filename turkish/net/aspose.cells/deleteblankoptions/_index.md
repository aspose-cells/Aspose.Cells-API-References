---
title: "Class DeleteBlankOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DeleteBlankOptions class. Boş hücreleri/satırları/sütunları silme ayarını temsil eder"
type: docs
url: /tr/net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

Boş hücreleri/satırları/sütunları silme ayarını temsil eder.

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | Resim, şekil, grafik gibi çizimle ilgili nesnelerin boş kabul edilip edilmeyeceğini gösterir. Varsayılan değer doğrudur. |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | Bir hücrenin formül olduğu ve hesaplanan sonucun null ya da boş dize olduğu durumda boş olarak kabul edilip edilmeyeceği. Varsayılan değer false. |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | Bir hücrenin değeri boş dize olduğunda boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer true. |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | Kontrol edilecek ve boş satırları/sütunları silinecek aralığın son satır/sütun indeksini (dahil) belirtir. Varsayılan değer -1'dir ve -1, kontrol edilmesi gereken tüm nesnelerin (hücreler, çizimler, ...) maksimum aralığını ifade eder. |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Silme işlemiyle oluşan değişiklikleri izlemek için monitörü alır/ayarlar. (Miras alınan [`DeleteOptions`](../deleteoptions/).) |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | Boş satırları/sütunları silerken birleştirilmiş hücrelerin nasıl işleneceğini gösterir. |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | Kontrol edilecek ve boş satır/sütun silinecek aralığın başlangıç satır/sütun indeksini belirtir. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. (Miras alınan [`DeleteOptions`](../deleteoptions/).) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteBlankOptionsDemo
    {
        public static void DeleteBlankOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasını bazı verilerle doldurun
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // DeleteBlankOptions sınıfının bir örneğini oluşturun
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true,
                EmptyFormulaValueAsBlank = false,
                UpdateReference = true
            };

            // Seçeneklere göre boş satırları sil
            worksheet.Cells.DeleteBlankRows(options);

            // Çalışma kitabını kaydedin
            workbook.Save("DeleteBlankOptionsExample.xlsx");
            workbook.Save("DeleteBlankOptionsExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


