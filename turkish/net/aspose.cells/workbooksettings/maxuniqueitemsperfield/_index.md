---
title: "WorkbookSettings.MaxUniqueItemsPerField"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Alan başına benzersiz öğe sınırlamasını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/maxuniqueitemsperfield/
---
## WorkbookSettings.MaxUniqueItemsPerField property

Alan başına benzersiz öğe sınırlamasını alır ve ayarlar.

```csharp
public int MaxUniqueItemsPerField { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertyMaxUniqueItemsPerFieldDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;

            try
            {
                // Mevcut MaxUniqueItemsPerField değerini göster
                Console.WriteLine("Current MaxUniqueItemsPerField value: " + settings.MaxUniqueItemsPerField);

                // MaxUniqueItemsPerField için yeni bir değer ayarlamayı gösterin
                settings.MaxUniqueItemsPerField = 1000;
                Console.WriteLine("After setting to 1000: " + settings.MaxUniqueItemsPerField);

                // Değiştirilebilir olduğunu göstermek için başka bir değer ayarlayın
                settings.MaxUniqueItemsPerField = 5000;
                Console.WriteLine("After setting to 5000: " + settings.MaxUniqueItemsPerField);

                // Örneği anlamlı kılmak için bazı örnek veriler ekleyin
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Orange");

                // Çalışma kitabını kaydedin
                workbook.Save("MaxUniqueItemsPerFieldDemo.xlsx");
                Console.WriteLine("Workbook saved with MaxUniqueItemsPerField settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


