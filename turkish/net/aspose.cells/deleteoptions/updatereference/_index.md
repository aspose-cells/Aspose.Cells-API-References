---
title: "DeleteOptions.UpdateReference"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DeleteOptions özelliği. Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/deleteoptions/updatereference/
---
## DeleteOptions.UpdateReference property

Diğer çalışma sayfalarındaki başvuruların güncellenip güncellenmeyeceğini gösterir.

```csharp
public bool UpdateReference { get; set; }
```

### Açıklamalar

26.7 sürümünden itibaren bu özelliğin varsayılan değerini true olarak ayarlıyoruz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ve formüller ekle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // UpdateReference özelliği true olarak ayarlanmış silme seçenekleri oluşturun
            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;

            // Formüllerde referans verilen A sütununu silin
            worksheet.Cells.DeleteColumns(0, 1, deleteOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


