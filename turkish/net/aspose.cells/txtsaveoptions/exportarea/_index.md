---
title: "TxtSaveOptions.ExportArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtSaveOptions özelliği. Dışa aktarılacak hücre aralığı"
type: docs
url: /tr/net/aspose.cells/txtsaveoptions/exportarea/
---
## TxtSaveOptions.ExportArea property

Aktarılacak hücre aralığı.

```csharp
public CellArea ExportArea { get; set; }
```

### Açıklamalar

Dışa aktarılan alan belirtilmişse, [`TrimLeadingBlankRowAndColumn`](../trimleadingblankrowandcolumn/) etkisiz olur.

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücreleri veri ile doldur
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(699.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(399.99);

            // ExportArea ile metin kaydetme seçeneklerini yapılandır
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = '\t',
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Yalnızca belirtilen alanı kaydet (ilk 3 satır, ilk 2 sütun)
            workbook.Save("ExportedData.txt", saveOptions);

            Console.WriteLine("Data exported successfully with ExportArea restriction.");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


