---
title: "InsertOptions.UpdateReference"
second_title: "Aspose.Cells için .NET API Referansı"
description: "InsertOptions özelliği. Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/insertoptions/updatereference/
---
## InsertOptions.UpdateReference property

Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir.

```csharp
public bool UpdateReference { get; set; }
```

### Açıklamalar

26.7 sürümünden itibaren bu özelliğin varsayılan değerini true olarak ayarlıyoruz.

### Örnekler

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İkinci bir çalışma sayfası ekleyin ve Sheet1'i referans alan formülleri ayarlayın
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].Formula = "=Sheet1!A10";
            sheet2.Cells["B1"].Formula = "=Sheet1!A5";
            
            // Sheet1'de formülleri ayarla
            Worksheet sheet1 = wb.Worksheets[0];
            sheet1.Cells["A1"].Formula = "=A10";
            sheet1.Cells["B1"].Formula = "=A5";

            // UpdateReference etkinleştirilmiş insert seçenekleri oluşturun
            InsertOptions iopts = new InsertOptions();
            iopts.UpdateReference = true;
            
            // Formül değişikliklerini izleyin
            HashSet<string> changedCells = new HashSet<string>();
            iopts.UpdateReference = true;
            
            // Formüllerdeki referansları güncelleyecek satırları ekleyin
            sheet1.Cells.InsertRows(5, 3, iopts);
            
            // Değişen hücre sayısını çıktı olarak verin
            Console.WriteLine("Formulas were automatically updated due to UpdateReference=true");
            
            // Güncellenen formülleri gösterin
            Console.WriteLine("Sheet1 A1 formula: " + sheet1.Cells["A1"].Formula);
            Console.WriteLine("Sheet2 A1 formula: " + sheet2.Cells["A1"].Formula);
        }
    }
}
```

### Ayrıca Bakınız

* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


