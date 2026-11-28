---
title: "ProtectedRange.CellArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ProtectedRange özelliği. Korunacak hücre alanını temsil eden CellArea nesnesini alır"
type: docs
url: /tr/net/aspose.cells/protectedrange/cellarea/
---
## ProtectedRange.CellArea property

Korunacak hücre alanını temsil eden `CellArea` nesnesini alır.

```csharp
public CellArea CellArea { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyCellAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Korunan aralıkları oluştur
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
            
            // İlk korunan aralığı ekle
            int index1 = allowRanges.Add("Range1", 0, 0, 2, 2);
            ProtectedRange range1 = allowRanges[index1];
            range1.Password = "123";

            // İkinci korunan aralığı ekle
            int index2 = allowRanges.Add("Range2", 3, 3, 5, 5);
            ProtectedRange range2 = allowRanges[index2];
            range2.Password = "456";

            // Her iki aralık için CellArea bilgisini göster
            Console.WriteLine("Protected Range 1:");
            Console.WriteLine($"Name: {range1.Name}");
            Console.WriteLine($"Area: {range1.CellArea.StartRow},{range1.CellArea.StartColumn} to {range1.CellArea.EndRow},{range1.CellArea.EndColumn}");

            Console.WriteLine("\nProtected Range 2:");
            Console.WriteLine($"Name: {range2.Name}");
            Console.WriteLine($"Area: {range2.CellArea.StartRow},{range2.CellArea.StartColumn} to {range2.CellArea.EndRow},{range2.CellArea.EndColumn}");

            // Çalışma kitabını kaydedin
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


