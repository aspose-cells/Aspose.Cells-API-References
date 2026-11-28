---
title: "CustomFilterCollection.And"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomFilterCollection özelliği. İki ölçütün AND ilişkisi olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/customfiltercollection/and/
---
## CustomFilterCollection.And property

İki ölçütün "and" ilişkisine sahip olup olmadığını gösterir.

```csharp
public bool And { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyAndDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Yeni bir CustomFilterCollection oluştur
                CustomFilterCollection filters = new CustomFilterCollection();

                // Varsayılan And özelliği değerini göster
                Console.WriteLine($"Default And property value: {filters.And}");

                // And özelliğini true olarak ayarla
                filters.And = true;
                Console.WriteLine($"After setting to true, And property value: {filters.And}");

                // And özelliğini false olarak ayarla
                filters.And = false;
                Console.WriteLine($"After setting to false, And property value: {filters.And}");

                // Çalışma kitabını kaydedin
                workbook.Save("CustomFilterCollectionAndDemo.xlsx");
                Console.WriteLine("CustomFilterCollection And property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating And property: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


