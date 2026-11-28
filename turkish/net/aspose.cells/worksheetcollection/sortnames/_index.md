---
title: "WorksheetCollection.SortNames"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Tanımlı adları sıralar"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/sortnames/
---
## WorksheetCollection.SortNames method

Tanımlı adları sıralar.

```csharp
public void SortNames()
```

### Açıklamalar

Excel dosyasında çok sayıda adlandırılmış aralık oluşturursanız, lütfen bu yöntemi tüm adlandırılmış aralıklar oluşturulduktan ve kaydetmeden önce çağırın

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSortNamesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı adlandırılmış aralıklar ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test1");
            worksheet.Cells.CreateRange("A1").Name = "Range2";
            worksheet.Cells["B1"].PutValue("Test2");
            worksheet.Cells.CreateRange("B1").Name = "Range1";
            
            // Sıralamadan önce adları göster
            Console.WriteLine("Before sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Adları sırala
            workbook.Worksheets.SortNames();
            
            // Sıralamadan sonra adları göster
            Console.WriteLine("\nAfter sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


