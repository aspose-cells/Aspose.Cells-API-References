---
title: "WorksheetCollection.GetNamedRanges"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Elektronik tabloda önceden tanımlanmış tüm adlandırılmış aralıkları alır"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/getnamedranges/
---
## WorksheetCollection.GetNamedRanges method

Elektronik tablodaki tüm önceden tanımlanmış adlandırılmış aralıkları alır.

```csharp
public Range[] GetNamedRanges()
```

### Dönüş Değeri

Range nesnelerinin bir dizisi. Tanımlı Adın referansı dışarıda ise veya birden fazla aralık içeriyorsa, bu Ad için hiçbir Range nesnesi döndürülmez.

Adlandırılmış aralık mevcut değilse null döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetNamedRangesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Gösterim için bazı adlandırılmış aralıklar oluşturun
            worksheet.Cells.CreateRange("A1:B2").Name = "SalesData";
            worksheet.Cells.CreateRange("C3:D4").Name = "Expenses";

            try
            {
                // Tüm adlandırılmış aralıkları almak için GetNamedRanges metodunu çağırın
                Aspose.Cells.Range[] namedRanges = workbook.Worksheets.GetNamedRanges();

                // Adlandırılmış aralıklar hakkında bilgileri gösterin
                Console.WriteLine("Found {0} named ranges:", namedRanges.Length);
                foreach (Aspose.Cells.Range range in namedRanges)
                {
                    Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
                }

                // Çalışma kitabını kaydedin
                workbook.Save("GetNamedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNamedRanges: {ex.Message}");
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


