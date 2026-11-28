---
title: "CustomFilter.SetCriteria"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomFilter yöntemi. Filtre kriterlerini ayarlar"
type: docs
url: /tr/net/aspose.cells/customfilter/setcriteria/
---
## CustomFilter.SetCriteria method

Filtre kriterini ayarlar.

```csharp
public void SetCriteria(FilterOperatorType filterOperator, object criteria)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filterOperator | FilterOperatorType | filtre operatör tipi |
| kriter | Object | filtre kriter değeri |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterMethodSetCriteriaWithFilterOperatorTObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);

            // Otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;

            try
            {
                // Bir özel filtre uygulayarak CustomFilter örneği elde edin
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Filtre koleksiyonundan ilk özel filtreyi alın
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // SetCriteria yöntemiyle kriterleri ayarla
                customFilter.SetCriteria(FilterOperatorType.GreaterThan, 25);

                // Ayarlanan kriterleri göster
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Çalışma kitabını kaydedin
                workbook.Save("SetCriteriaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


