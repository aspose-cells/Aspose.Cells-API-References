---
title: "SaveOptions.SortNames"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SaveOptions özelliği. Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/saveoptions/sortnames/
---
## SaveOptions.SortNames property

Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir.

```csharp
public bool SortNames { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySortNamesDemo
    {
        public static void Run()
        {
            // Yeni bir Workbook nesnesi oluştur
            Workbook workbook = new Workbook();
            
            // Örnek veri ekleyin.
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Adlandırılmış bir aralık oluştur
            worksheet.Cells.CreateRange("A2:B3").Name = "MyDataRange";

            // SortNames etkinleştirilmiş şekilde kaydetme seçenekleri oluşturun
            XlsSaveOptions saveOptions = new XlsSaveOptions
            {
                SortNames = true
            };

            // Çalışma kitabını kaydedin
            workbook.Save("SortedNamesExample.xls", saveOptions);

            Console.WriteLine("Workbook saved with sorted named ranges.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


