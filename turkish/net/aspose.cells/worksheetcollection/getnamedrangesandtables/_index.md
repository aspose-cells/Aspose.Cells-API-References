---
title: "WorksheetCollection.GetNamedRangesAndTables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Elektronik tabloda önceden tanımlanmış tüm adlandırılmış aralıkları alır"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/getnamedrangesandtables/
---
## WorksheetCollection.GetNamedRangesAndTables method

Elektronik tablodaki tüm önceden tanımlanmış adlandırılmış aralıkları alır.

```csharp
public Range[] GetNamedRangesAndTables()
```

### Dönüş Değeri

Range nesnelerinden oluşan bir dizi.

Adlandırılmış aralık mevcut değilse null döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetNamedRangesAndTablesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı adlandırılmış aralıklar oluştur
            worksheet.Cells.CreateRange("A1:B2").Name = "TestRange1";
            worksheet.Cells.CreateRange("C3:D4").Name = "TestRange2";
            
            // Tüm adlandırılmış aralıkları ve tabloları al
            Aspose.Cells.Range[] ranges = workbook.Worksheets.GetNamedRangesAndTables();
            
            // Aralıklar hakkında bilgiyi göster
            Console.WriteLine("Found {0} named ranges:", ranges.Length);
            foreach (Aspose.Cells.Range range in ranges)
            {
                Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


