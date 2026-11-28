---
title: "DeleteBlankOptions.EmptyStringAsBlank"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DeleteBlankOptions özelliği. Bir hücrenin değeri boş bir dize olduğunda boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer true'tir."
type: docs
url: /tr/net/aspose.cells/deleteblankoptions/emptystringasblank/
---
## DeleteBlankOptions.EmptyStringAsBlank property

Bir hücrenin değeri boş dize olduğunda boş olarak kabul edilip edilmeyeceğini gösterir. Varsayılan değer true.

```csharp
public bool EmptyStringAsBlank { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyStringAsBlankDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Boş dizeler dahil olmak üzere veriyle çalışma sayfasını doldur
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // DeleteBlankOptions'ı EmptyStringAsBlank true olarak ayarlayarak yapılandır
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true
            };

            // Boş dizeler içeren satırları sil (boş olarak kabul edilir)
            worksheet.Cells.DeleteBlankRows(options);

            // Sonucu kaydet
            workbook.Save("DeleteBlankOptions_EmptyStringAsBlank_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


