---
title: "AutoFitterOptions.AutoFitMergedCellsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFitterOptions özelliği. Birleştirilmiş hücrelerin satır yüksekliğini otomatik sığdırma türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/autofitteroptions/autofitmergedcellstype/
---
## AutoFitterOptions.AutoFitMergedCellsType property

Birleştirilmiş hücrelerin satır yüksekliğinin otomatik ayarlanma türünü alır ve ayarlar.

```csharp
public AutoFitMergedCellsType AutoFitMergedCellsType { get; set; }
```

### Açıklamalar

Excel, satır yüksekliğini ayarlarken birleştirilmiş hücreleri yok saymayı varsayılan olarak alır, bu yüzden Aspose.Cells MS Excel varsayılanı gibi çalışır. Lütfen bu türü ayarlayarak birleştirilmiş hücrelerin satır yüksekliğini otomatik sığdırma şeklini değiştirin.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek verileri ayarlayın ve hücreleri birleştirin
            worksheet.Cells["A1"].PutValue("This is a sample text for merged cells auto-fit demonstration");
            worksheet.Cells.Merge(0, 0, 3, 2); // Merge A1:B3

            // AutoFitMergedCellsType.EachLine ile satırları otomatik sığdırın
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // AutoFitMergedCellsType.EachLine ile sütunları otomatik sığdırın
            worksheet.AutoFitColumns(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitMergedCellsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [AutoFitMergedCellsType](../../autofitmergedcellstype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


