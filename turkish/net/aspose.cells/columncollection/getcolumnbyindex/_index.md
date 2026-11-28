---
title: "ColumnCollection.GetColumnByIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ColumnCollection yöntemi. Listedeki konuma göre Column nesnesini alır"
type: docs
url: /tr/net/aspose.cells/columncollection/getcolumnbyindex/
---
## ColumnCollection.GetColumnByIndex method

Listedeki konuma göre [`Column`](../../column/) nesnesini alır.

```csharp
public Column GetColumnByIndex(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Listedeki konum. |

### Dönüş Değeri

Sütun nesnesini döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetColumnByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A sütununa örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Aspose.Cells Column Demo";

            try
            {
                // Sütun koleksiyonu referansını alın
                ColumnCollection columns = worksheet.Cells.Columns;

                // GetColumnByIndex kullanarak indeks 0'da (A sütunu) sütuna erişin
                Column column = columns.GetColumnByIndex(0);

                // Sütun erişimini göstermek için sütun genişliğini değiştirin
                column.Width = 25;

                Console.WriteLine("Modified width of column at index 0 (Column A) to 25 characters.");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid column index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("ColumnCollectionMethodGetColumnByIndexWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


