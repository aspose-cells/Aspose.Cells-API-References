---
title: "ListObject.HasAutoFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Bu tabloya otomatik filtre uygulanıp uygulanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.tables/listobject/hasautofilter/
---
## ListObject.HasAutoFilter property

Otomatik filtrenin bu tabloya uygulanıp uygulanmadığını gösterir.

```csharp
public bool HasAutoFilter { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Tables;

    public class ListObjectPropertyHasAutoFilterDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tablo için örnek verileri doldur
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Charlie");
            worksheet.Cells["B4"].PutValue(78);

            try
            {
                // Veri aralığını kapsayan bir ListObject (tablo) ekle
                int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[tableIndex];

                // Tablonun tüm satırları içerecek şekilde yeniden boyutlandırıldığından emin ol
                listObject.Resize(0, 0, 4, 2, true);

                // HasAutoFilter özelliği değerini oku ve göster
                bool hasFilter = listObject.HasAutoFilter;
                Console.WriteLine("HasAutoFilter: " + hasFilter);

                // AutoFilter nesnesine AutoFilter özelliği üzerinden erişilebilir
                // HasAutoFilter true olduğunda nesnenin null olmadığını göster
                if (hasFilter && listObject.AutoFilter != null)
                {
                    // "Score" sütununda (indeks 1) basit bir filtre uygulayarak Score >= 80 olan satırları göster
                    listObject.AutoFilter.Filter(1, ">=80");

                    Console.WriteLine("Filtered rows (Score >= 80):");
                    for (int row = 1; row <= 4; row++)
                    {
                        // Satırın gizli olup olmadığını kontrol etmek için Cells.Rows kullan
                        if (!worksheet.Cells.Rows[row].IsHidden)
                        {
                            Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                        }
                    }

                    // Filtreyi temizle
                    listObject.AutoFilter.RemoveFilter(1);
                }

                // Çalışma kitabını kaydedin (isteğe bağlı)
                workbook.Save("HasAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


