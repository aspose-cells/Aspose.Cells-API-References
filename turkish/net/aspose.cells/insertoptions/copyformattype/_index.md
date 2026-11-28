---
title: "InsertOptions.CopyFormatType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "InsertOptions özelliği."
type: docs
url: /tr/net/aspose.cells/insertoptions/copyformattype/
---
## InsertOptions.CopyFormatType property

```csharp
public CopyFormatType CopyFormatType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyCopyFormatTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrasyon için değerleri ve biçimlendirmeyi ayarlayın
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");

            // InsertOptions oluşturun ve CopyFormatType'ı ayarlayın
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.SameAsAbove;

            // Yukarıdaki biçimlendirmeyle bir satır ekleyin
            worksheet.Cells.InsertRows(2, 1, options);

            // Sonucu kaydet
            workbook.Save("InsertWithFormatting.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


