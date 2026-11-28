---
title: "NameCollection.RemoveDuplicateNames"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NameCollection yöntemi. Yinelenen tanımlı adları kaldır"
type: docs
url: /tr/net/aspose.cells/namecollection/removeduplicatenames/
---
## NameCollection.RemoveDuplicateNames method

Tanımlı yinelenen isimleri kaldır.

```csharp
public void RemoveDuplicateNames()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveDuplicateNamesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yinelenen adlarla bazı adlandırılmış aralıklar ekle
            worksheet.Cells["A1"].PutValue("Test Value 1");
            worksheet.Cells["B1"].PutValue("Test Value 2");
            
            // Doğru Add yöntemi imzasını kullanarak yinelenen adlandırılmış aralıklar oluştur
            int index1 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$B$1";
            
            // Yinelenenleri kaldırmadan önce sayıyı göster
            Console.WriteLine($"Named ranges count before removal: {workbook.Worksheets.Names.Count}");
            
            // Yinelenen adları kaldır
            workbook.Worksheets.Names.RemoveDuplicateNames();
            
            // Yinelenenleri kaldırdıktan sonra sayıyı göster
            Console.WriteLine($"Named ranges count after removal: {workbook.Worksheets.Names.Count}");
        }
    }
}
```

### Ayrıca Bakınız

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


