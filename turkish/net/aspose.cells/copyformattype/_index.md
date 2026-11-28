---
title: "Enum CopyFormatType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CopyFormatType enum. Satır eklerken kopyalama biçiminin türünü temsil eder."
type: docs
url: /tr/net/aspose.cells/copyformattype/
---
## CopyFormatType enumeration

Satır eklerken kopyalama biçimi türünü temsil eder.

```csharp
public enum CopyFormatType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| SameAsAbove | `0` | Biçimler yukarıdaki satırla aynı. |
| SameAsBelow | `1` | Biçimler aşağıdaki satırla aynı. |
| Clear | `2` | Biçimlendirmeyi temizler. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CopyFormatTypeDemo
    {
        public static void CopyFormatTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı verileri doldurun
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");

            // InsertOptions oluşturun ve CopyFormatType'ı ayarlayın
            InsertOptions insertOptions = new InsertOptions();
            insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;

            // Belirtilen biçim türüyle ikinci konuma bir satır ekleyin
            worksheet.Cells.InsertRows(1, 1, insertOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("CopyFormatTypeExample.xlsx");
            workbook.Save("CopyFormatTypeExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


