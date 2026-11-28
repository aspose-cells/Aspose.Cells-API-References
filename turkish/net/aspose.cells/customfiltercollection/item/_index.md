---
title: "CustomFilterCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomFilterCollection özelliği. Belirli indeksteki özel filtreyi alır"
type: docs
url: /tr/net/aspose.cells/customfiltercollection/item/
---
## CustomFilterCollection indexer

Belirli indeksteki özel filtreyi alır.

```csharp
public CustomFilter this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyItemDemo
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

                // İndeksleyici kullanarak Item özelliğine (yalnızca okunabilir) eriş
                // Koleksiyon boş olduğu için, sadece özelliğe erişimi göstereceğiz
                // Gerçek bir senaryoda, önce filtreleri başka yollarla eklerdiniz
                if (filters.Count > 0)
                {
                    CustomFilter firstFilter = filters[0];
                    Console.WriteLine($"First filter operator: {firstFilter.FilterOperatorType}");
                    Console.WriteLine($"First filter criteria: {firstFilter.Criteria}");
                }
                else
                {
                    Console.WriteLine("No filters in collection to demonstrate Item property");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("CustomFilterCollectionItemDemo.xlsx");
                Console.WriteLine("CustomFilterCollection Item property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomFilter](../../customfilter/)
* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


