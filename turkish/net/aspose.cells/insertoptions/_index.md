---
title: "Sınıf InsertOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.InsertOptions sınıfı. Ekleme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/insertoptions/
---
## InsertOptions class

Ekleme seçeneklerini temsil eder.

```csharp
public class InsertOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [InsertOptions](insertoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CopyFormatType](../../aspose.cells/insertoptions/copyformattype/) { get; set; } |  |
| [FormulaChangeMonitor](../../aspose.cells/insertoptions/formulachangemonitor/) { get; set; } | Ekleme nedeniyle oluşan değişiklikleri izlemek için monitörü alır/ayarlar. |
| [UpdateReference](../../aspose.cells/insertoptions/updatereference/) { get; set; } | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsDemo
    {
        public static void InsertOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // InsertOptions bir örnek oluşturun
            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Satırların ekleneceği hücre alanını tanımlayın
            CellArea cellArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };

            // Belirtilen seçeneklerle satırları ekleyin
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("InsertOptionsExample.xlsx");
            workbook.Save("InsertOptionsExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


