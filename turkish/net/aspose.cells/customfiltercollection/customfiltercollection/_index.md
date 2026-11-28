---
title: "CustomFilterCollection.CustomFilterCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomFilterCollection yapıcı. Yeni bir örnek oluşturur"
type: docs
url: /tr/net/aspose.cells/customfiltercollection/customfiltercollection/
---
## CustomFilterCollection constructor

Yeni bir örnek oluşturur.

```csharp
[Obsolete("Use FilterColumn.CustomFilters, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomFilterCollection()
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, FilterColumn.FilterType'ı FilterType.CustomFilters olarak ayarlayın ve ardından FilterColumn.CustomFilters'ı alın. Bu özellik, Haziran 2026'dan itibaren 12 ay içinde kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionMethodSharpctorDemo
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
                // Yapıcıyı kullanarak yeni bir CustomFilterCollection oluştur
                CustomFilterCollection filters = new CustomFilterCollection();

                // Varsayılan And özelliği değerini göster
                Console.WriteLine($"Default And property value: {filters.And}");

                // Yapıcı boş bir koleksiyon oluşturur
                Console.WriteLine($"Number of filters in collection: {filters.Count}");

                // Çalışma kitabını kaydedin
                workbook.Save("CustomFilterCollectionDemo.xlsx");
                Console.WriteLine("CustomFilterCollection created successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomFilterCollection: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


