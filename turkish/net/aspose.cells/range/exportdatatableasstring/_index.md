---
title: "Range.ExportDataTableAsString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Bu aralıktaki verileri bir DataTable nesnesine dışa aktarır"
type: docs
url: /tr/net/aspose.cells/range/exportdatatableasstring/
---
## Range.ExportDataTableAsString method

Bu aralıktaki verileri bir DataTable nesnesine dışa aktarır.

```csharp
public DataTable ExportDataTableAsString()
```

### Dönüş Değeri

Dışa aktarılmış DataTable nesnesi.

### Açıklamalar

[`Cells`](../../cells/) koleksiyonundaki tüm veriler stringe dönüştürülür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class RangeMethodExportDataTableAsStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(30);

            // Verileri içeren aralığı al
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            try
            {
                // ExportDataTableAsString yöntemini çağır
                DataTable dataTable = range.ExportDataTableAsString();

                // Dışa aktarılan verileri görüntüle
                Console.WriteLine("Exported DataTable:");
                foreach (DataRow row in dataTable.Rows)
                {
                    Console.WriteLine($"{row[0]}, {row[1]}");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RangeMethodExportDataTableAsStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportDataTableAsString method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


